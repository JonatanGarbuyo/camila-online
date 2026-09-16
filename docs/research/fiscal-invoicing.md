# Facturación y titularidad del canal online

_Verificado: 2026-09-16._

> Research operativo. No guardar CUIT, claves fiscales ni credenciales en este repositorio.

## Facturación electrónica

ARCA publica que monotributistas de todas las categorías deben emitir comprobantes electrónicos tipo `C` por sus operaciones con consumidores finales. Para responsables inscriptos, la clase del comprobante depende del receptor; frente a consumidor final normalmente corresponde comprobante `B`.

ARCA ofrece mecanismos como `Comprobantes en línea` y herramientas de facturación electrónica. Por lo tanto, **la venta online no elimina la obligación de facturar**: debe incorporarse al circuito fiscal del comercio que realiza la venta.

Fuentes oficiales:
- https://www.arca.gob.ar/facturacion/monotributo/comprobantes.asp
- https://www.arca.gob.ar/monotributo/ayuda/facturacion.asp
- https://www.arca.gob.ar/facturacion/regimen-general/
- https://www.arca.gob.ar/fe/emision-autorizacion/sujetos.asp

## Tiendanube y facturación

Tiendanube permite facturar de forma manual mediante ARCA o instalar aplicaciones de facturación. Su documentación lista herramientas como Facturante, iFactura, Contabilium y otras.

Para ventas cobradas con **Pago Nube**, Tiendanube indica que la facturación automática actualmente está disponible con **Facturante**; con otras aplicaciones puede requerirse gestión manual. Facturante ofrece prueba y luego puede implicar un costo adicional.

Fuentes:
- https://ayuda.tiendanube.com/es_AR/123288-mis-ventas/como-facturar-las-ventas-de-mi-tiendanube
- https://ayuda.tiendanube.com/es_AR/123502-aplicaciones-de-gestion-y-facturacion/como-integrar-facturante-con-mi-tienda
- https://ayuda.tiendanube.com/es_AR/123482-planes/en-que-planes-puedo-instalar-aplicaciones-en-mi-tiendanube

## Implicación para el MVP de costo bajo

La automatización fiscal **no tiene que ser requisito del día uno** si el comercio ya posee un circuito de facturación y el volumen inicial es bajo. Se puede incorporar manualmente el pedido online a ese circuito.

Esto debe validarse con Camila:

- quién o qué entidad factura hoy las ventas del negocio;
- qué sistema/herramienta usan actualmente;
- si las ventas del local ya descuentan stock desde ese sistema;
- quién emite el comprobante y en qué momento;
- si el trabajo manual de sumar pedidos online sería aceptable al inicio.

No pedir ni registrar CUIT, clave fiscal, tokens ni credenciales.

## Titularidad propuesta del canal

### Propuesta

El **comercio físico / sus dueños** deberían ser titulares de las cuentas que representan al vendedor y reciben dinero, por ejemplo:

- cuenta principal de la tienda online;
- Pago Nube / medio de cobro;
- datos fiscales y facturación;
- relación contractual con operadores de envío cuando corresponda.

Camila debería operar como **administradora del canal online**, con acceso delegado cuando la plataforma lo permita, y cobrar su servicio de administración por separado.

### Motivo

Esta separación reduce problemas de continuidad, conciliación y responsabilidad: si Camila deja de administrar la tienda, el comercio conserva clientes, pedidos, cobros y cuentas. También evita mezclar ingresos del comercio con ingresos personales de Camila.

Esta es una **propuesta de arquitectura comercial**, no una decisión final aprobada. Debe validarse con Camila y los dueños, y la decisión final corresponde a `@JonatanGarbuyo`.

## Restricción del plan Inicial

Tiendanube Inicial permite múltiples usuarios, pero **sin permisos diferenciados**: los usuarios administradores tienen acceso total. Esto debe evaluarse si los dueños quieren dar acceso operativo a Camila sin exponer todas las funciones administrativas.

Fuente:
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube

## Pregunta abierta

¿El esquema de acceso total del plan Inicial es aceptable para el primer comercio? Si no lo es, puede convertirse en un motivo concreto para usar un plan pago u otra plataforma.