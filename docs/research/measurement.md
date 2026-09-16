# Métricas, atribución y observabilidad

_Verificado: 2026-09-16._

## Conclusión de research

El MVP puede medir adquisición y ventas **sin costo fijo adicional** usando:

1. UTMs consistentes en todos los links externos;
2. integración nativa de GA4;
3. integración nativa de Meta Pixel + Conversion API;
4. reporting semanal simple del funnel y costos operativos.

No hace falta montar infraestructura de observabilidad técnica ni Google Tag Manager para los eventos estándar del e-commerce. Tiendanube documenta que ya envía los eventos relevantes mediante sus integraciones nativas y advierte que duplicarlos con GTM puede contaminar las métricas.

## Objetivo mínimo

Poder responder:

1. ¿Cuántas personas llegaron desde Instagram, Facebook, WhatsApp o un referido?
2. ¿Qué publicación/campaña/link generó la visita?
3. ¿Cuántas avanzaron hacia checkout?
4. ¿Cuántas compraron?
5. ¿Cuánto vendió cada fuente/campaña?

## 1. UTM en todos los links publicados

Convención propuesta:

- `utm_source`: `instagram`, `facebook`, `whatsapp`, `referral`
- `utm_medium`: `organic_social`, `paid_social`, `message`, `referral`
- `utm_campaign`: nombre estable de campaña
- `utm_content`: `bio`, `story`, `reel`, `post`, creador/referidor o variante

Google Analytics documenta estos parámetros para identificar campañas y verlas en adquisición de tráfico.

Fuente primaria:
- https://support.google.com/analytics/answer/10917952

Ejemplo:

`https://marca.mitiendanube.com/?utm_source=instagram&utm_medium=organic_social&utm_campaign=lanzamiento&utm_content=bio`

### Regla operativa

**No publicar un link comercial sin atribución.**

Para referidos individuales, usar un identificador estable en `utm_content` o una campaña específica si se quiere comparar referidores.

## 2. GA4

El plan Inicial de Tiendanube incluye integración con Google Analytics.

Tiendanube documenta que su integración nativa envía, entre otros:

- `view_item_list`
- `select_item`
- `view_item`
- `add_to_cart`
- `remove_from_cart`
- `view_cart`
- `begin_checkout`
- `add_payment_info`
- `purchase`

Google recomienda estos eventos estándar para análisis de e-commerce y funnel.

Fuentes primarias:
- https://ayuda.tiendanube.com/es_AR/google-analytics/como-vincular-google-analytics-4-con-mi-tiendanube
- https://ayuda.tiendanube.com/es_AR/google/como-instalar-google-tag-manager-en-mi-tiendanube
- https://support.google.com/analytics/answer/9267735?hl=es

## 3. Meta Pixel + Conversion API

El plan Inicial soporta Pixel y API de conversiones de Meta.

La integración nativa de Tiendanube envía desde servidor los eventos:

- Agregar al carrito;
- Agregar información de pago;
- Comprar.

Tiendanube documenta que el evento de compra del backend puede dispararse cuando la orden está efectivamente paga, reduciendo falsos positivos de conversiones.

Fuente primaria:
- https://ayuda.tiendanube.com/es_AR/pixel-de-facebook/como-activar-la-api-de-conversiones-de-facebook

## 4. No agregar GTM al MVP para eventos estándar

Tiendanube ya envía los eventos principales a GA4/Google Ads y recomienda no duplicarlos vía Google Tag Manager porque puede generar mediciones duplicadas.

Usar GTM solamente si en el futuro aparece un evento específico que las integraciones nativas no cubren.

Fuente:
- https://ayuda.tiendanube.com/es_AR/google/como-instalar-google-tag-manager-en-mi-tiendanube

## Reporting mínimo semanal

### Adquisición

- sesiones por `source / medium`;
- sesiones por `campaign / content`;
- links/campañas que generan tráfico.

### Funnel

- vistas de producto;
- add-to-cart;
- begin-checkout;
- purchase;
- tasa visita → compra;
- tasa checkout → compra.

### Negocio

- revenue total;
- revenue por fuente/campaña cuando la atribución esté disponible;
- ticket promedio;
- costo de pago por venta;
- costo de envío/seguro por venta;
- cambios/devoluciones;
- pedidos pendientes/demorados.

## Referidos

Para medir el impacto de una persona o comercio que comparte la tienda:

- generar un link con `utm_source=referral`;
- `utm_medium=referral`;
- `utm_campaign=<campaña>`;
- `utm_content=<id_referidor>`.

No hace falta construir un sistema de afiliados en el MVP. Si más adelante hay comisión económica por referido, eso será otra decisión porque requiere reglas de atribución, ventana temporal y conciliación.

## Observabilidad

Para un MVP no-code, “observabilidad” significa observar **negocio + operación**, no montar logs/APM/tracing.

Monitorear:

- tienda y checkout funcionales;
- errores/rechazos de pago;
- pedidos pendientes de despacho;
- entregas demoradas o siniestradas;
- discrepancias de stock/precio;
- cambios/devoluciones;
- caída anormal de conversión.

Infraestructura técnica de observabilidad queda fuera mientras no exista software propio.

## Riesgo de atribución

Si una venta sale del checkout y termina cerrándose manualmente por WhatsApp o un Link de Pago externo, se puede perder la atribución automática de revenue.

Por eso:

- el checkout integrado debe seguir siendo el camino principal;
- las ventas asistidas deben registrar manualmente al menos `source/campaign/referrer` si se quiere preservar la medición.
