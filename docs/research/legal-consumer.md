# Obligaciones de consumo: arrepentimiento, devoluciones y reintegros

_Verificado: 2026-09-16._

> Research operativo para el proyecto. No reemplaza asesoramiento legal individual.

## Derecho de arrepentimiento en ventas online

Para ventas a distancia en Argentina, la Ley 24.240 (texto actualizado), artículo 34, establece un plazo de **10 días corridos** para revocar la aceptación, contado desde la entrega del bien o la celebración del contrato, lo último que ocurra. La facultad no puede renunciarse y **los gastos de devolución son a cargo del vendedor**.

El Código Civil y Comercial, artículos 1110 a 1115, también regula la revocación en contratos a distancia y establece que el ejercicio del derecho no debe implicar gasto para el consumidor.

Fuentes oficiales:
- https://www.argentina.gob.ar/normativa/nacional/638/actualizacion
- https://www.argentina.gob.ar/normativa/nacional/235975/texto

## Botón de arrepentimiento

La norma reglamentaria vigente es la **Disposición 954/2025**, que reemplazó a la Resolución 424/2020. Exige que los proveedores que venden a distancia tengan un link denominado `BOTÓN DE ARREPENTIMIENTO` a simple vista, en lugar destacado y en el primer acceso, sin exigir registración previa ni trámites adicionales para iniciar la solicitud.

La Disposición 3/2026 aclaró que pueden existir pasos razonables de verificación de identidad con finalidad de seguridad.

Fuentes oficiales:
- https://www.argentina.gob.ar/normativa/nacional/norma-417152/texto
- https://www.argentina.gob.ar/normativa/nacional/disposici%C3%B3n-3-2026-423007/texto

## Qué resuelve Tiendanube

Tiendanube incorpora un botón de arrepentimiento para tiendas argentinas. Su documentación indica que:

- el cliente completa un formulario y obtiene un número de reclamo;
- el comercio recibe la solicitud en el administrador/email;
- la orden **no se cancela automáticamente**: hay que gestionarla;
- Pago Nube permite reembolsos totales o parciales al medio de pago correspondiente.

Fuentes:
- https://ayuda.tiendanube.com/es_AR/123288-mis-ventas/que-es-el-boton-de-arrepentimiento-de-compra-de-mi-tiendanube
- https://ayuda.tiendanube.com/es_AR/pago-nube/como-devolver-el-pago-de-mi-cliente-a-traves-de-pago-nube

## Punto de verificación antes de lanzar

La documentación de Tiendanube actualizada en 2026 todavía referencia la Resolución 424/2020 —derogada por la Disposición 954/2025— y describe el botón en el pie de página. La norma vigente exige que esté visible y destacado en el primer acceso.

Esto **no alcanza para concluir que Tiendanube incumple**: puede haber diferencias entre documentación e implementación o criterios de visualización. Pero debe verificarse en una tienda real antes del lanzamiento y, si hay duda, consultarse a Tiendanube o asesor legal.

## Diferenciar dos flujos

### 1. Arrepentimiento legal

Es el derecho regulado para compras a distancia. El comercio debe prever devolución/reintegro y el costo de devolución puede recaer en el vendedor conforme a la normativa indicada.

### 2. Cambio comercial por talle/color

Es una política operativa/comercial distinta. En indumentaria puede ser frecuente aunque el cliente no quiera deshacer la compra sino cambiar la variante.

El proyecto debe diseñar ambos casos por separado para evitar confundir una obligación legal con una política voluntaria de cambios.

## Implicación para Camila Online

El costo y la operación de devoluciones **no pueden modelarse como cero**, aunque el volumen inicial sea bajo. El plan Inicial no ofrece logística reversa integrada, por lo que el flujo de devolución/cambio deberá resolverse operativamente fuera de la automatización de envío inicial.

Esto alimenta el ticket #8 (cambios, devoluciones y logística inversa).