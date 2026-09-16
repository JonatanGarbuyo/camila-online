# Métricas, atribución y observabilidad

_Verificado: 2026-09-16._

## Objetivo mínimo

Poder responder:

1. ¿Cuántas personas llegaron desde Instagram, Facebook, WhatsApp o un referido?
2. ¿Qué publicación/campaña/link generó la visita?
3. ¿Cuántas avanzaron hacia checkout?
4. ¿Cuántas compraron?
5. ¿Cuánto vendió cada fuente/campaña?

## Stack mínimo sin costo fijo

### 1. UTM en todos los links publicados

Convención propuesta:

- `utm_source`: `instagram`, `facebook`, `whatsapp`, `referral`
- `utm_medium`: `organic_social`, `paid_social`, `message`, `referral`
- `utm_campaign`: nombre estable de campaña
- `utm_content`: `bio`, `story`, `reel`, `post`, creador/referidor o variante

Google Analytics documenta estos parámetros para identificar campañas y verlas en los reportes de adquisición.

Fuente primaria:
- https://support.google.com/analytics/answer/10917952

Ejemplo:

`https://marca.mitiendanube.com/?utm_source=instagram&utm_medium=organic_social&utm_campaign=lanzamiento&utm_content=bio`

### 2. GA4

El plan Inicial de Tiendanube publica integración con Google Analytics.

Fuente:
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube

### 3. Meta

El mismo plan publica soporte para Pixel y API de conversiones de Facebook. Esto es particularmente útil si Facebook/Instagram son canales de adquisición importantes.

Fuente:
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube

## Regla operativa

**No publicar un link comercial sin atribución.**

Para links orgánicos/sociales: UTM.
Para referidos individuales: usar además un identificador estable en `utm_content` o `utm_campaign` según el modelo elegido.

Ejemplos:

- Bio IG: `source=instagram / medium=organic_social / campaign=lanzamiento / content=bio`
- Story producto: `source=instagram / medium=organic_social / campaign=lanzamiento / content=story_campera_01`
- Referido de Ana: `source=referral / medium=referral / campaign=lanzamiento / content=ana`

## Reporting mínimo semanal

- sesiones por source/medium;
- sesiones por campaign/content;
- pedidos/ventas;
- revenue total;
- revenue por fuente/campaña si la plataforma/analytics preserva la atribución;
- tasa visita → compra;
- ticket promedio;
- costo de pago por venta;
- costo de envío/seguro por venta;
- cambios/devoluciones;
- conversaciones de WhatsApp originadas desde la tienda, si se puede medir sin complejidad excesiva.

## Observabilidad

Para un MVP no-code, “observabilidad” no debe convertirse en montar infraestructura técnica.

Lo útil inicialmente es observar el **negocio y el funnel**:

- tienda disponible y checkout funcional;
- errores/reclamos de pago;
- pedidos pendientes de despacho;
- entregas demoradas o siniestradas;
- abandono del funnel;
- discrepancias de stock/precio;
- cambios/devoluciones.

Logs, APM y tracing técnico quedan fuera mientras no haya software propio.

## Riesgo de atribución

Si una venta abandona el checkout y termina cerrándose manualmente por WhatsApp o Link de Pago externo, la atribución automática puede cortarse.

Por eso la venta autoservicio integrada es preferible como camino principal. Cuando haya venta asistida, conviene registrar al menos `source/campaign/referrer` junto al pedido o contacto.
