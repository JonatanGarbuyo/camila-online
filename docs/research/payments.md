# Pagos online

_Verificado: 2026-09-16._

## Conclusión de research

**Pago Nube no bloquea el MVP de Tiendanube Inicial.** Cubre el set mínimo que necesitamos para una venta autoservicio: tarjeta de crédito/débito, MODO y transferencia, administrados dentro del checkout de la tienda.

La estrategia inicial recomendada es:

1. ofrecer tarjeta/débito/MODO para no sacrificar conversión;
2. ofrecer transferencia como opción de menor costo;
3. usar **14 días de liberación** como default orientado a costo si el flujo de caja del negocio lo tolera;
4. pasar a 7 días si la operación demuestra que necesita liquidez más rápida;
5. no activar cuotas sin interés por defecto hasta conocer margen/ticket, porque agregan costo de financiación.

El plazo de liberación es una configuración reversible; no requiere una decisión arquitectónica irreversible.

## Pago Nube en Tiendanube Inicial

Tarifas publicadas para el plan Inicial al 04/08/2026:

- tarjetas de crédito/débito y MODO, liberación en 1 día: **6,40% + IVA**;
- liberación en 7 días: **4,45% + IVA**;
- liberación en 14 días: **3,50% + IVA**;
- transferencia: **1,50% + IVA**.

En ventas cobradas con Pago Nube, Tiendanube publica costo por transacción de plataforma bonificado al 0%.

La comisión de Pago Nube se calcula sobre el total de la orden, incluyendo el envío.

El plan Inicial solo permite Pago Nube como medio de pago integrado.

Pago Nube no genera links de pago externos: opera dentro del checkout de la tienda. Para el proyecto esto es aceptable, porque el checkout integrado es el camino principal y WhatsApp es asistencia.

Fuentes primarias:
- https://ayuda.tiendanube.com/es_AR/pago-nube/cuales-son-las-comisiones-de-pago-nube
- https://ayuda.tiendanube.com/es_AR/pago-nube/que-es-pago-nube
- https://ayuda.tiendanube.com/es_AR/123484-costos-por-transaccion/como-se-calculan-los-costos-por-transaccion
- https://ayuda.tiendanube.com/es_AR/122919-informacion/cuales-son-las-aplicaciones-de-pagos-disponibles-para-tiendanube

## Comparación con Mercado Pago

Mercado Pago Checkout/Link publica:

- acreditación inmediata: **6,29% + IVA**;
- 10 días: **4,39% + IVA**;
- 18 días: **3,39% + IVA**;
- 35 días: **1,49% + IVA**.

Las diferencias de tasa frente a Pago Nube son pequeñas en plazos comparables. Para una tienda en validación, el ahorro de costo fijo de Tiendanube Inicial pesa más que una diferencia marginal de comisión, salvo que aparezca una necesidad concreta de Mercado Pago u otro medio.

Empretienda permite Mercado Pago, Ualá Bis, transferencia y otros medios sin comisión de plataforma, pero agrega su abono mensual.

Fuentes primarias:
- https://www.mercadopago.com.ar/herramientas-para-vender/check-out
- https://www.mercadopago.com.ar/herramientas-para-vender/link-de-pago
- https://api.empretienda.com/

## Impuestos y retenciones

La tasa de la pasarela no es necesariamente el costo financiero total. Pago Nube documenta IVA sobre comisiones y posibles percepciones/retenciones según la situación fiscal, incluyendo IIBB/SIRTAC cuando corresponda.

Esto debe validarse con la situación fiscal real del negocio antes de construir una proyección de margen.

Fuente primaria:
- https://ayuda.tiendanube.com/pago-nube-2/que-costos-debo-tener-en-cuenta-al-vender-con-pago-nube

## Regla para el MVP

No optimizar centésimas de comisión sacrificando el checkout integrado.

Medir desde el lanzamiento:

- proporción tarjeta vs transferencia;
- comisión efectiva por venta;
- tiempo real hasta disponibilidad de fondos;
- uso de cuotas;
- abandono/rechazos de pago;
- impacto del costo financiero sobre margen.

Revisar el plazo de liberación cuando existan datos reales.
