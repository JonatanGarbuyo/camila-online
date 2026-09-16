# DonWeb SitioSimple — evaluación para el MVP

[← Índice de investigación](README.md) · [Shortlist](shortlist-plataformas.md) · [Protocolo #19](protocolo-prueba-plataformas.md) · [Índice general](../INDEX.md)

_Verificado: 2026-09-16._

## Estado

**Candidato activo, no decisión final.**

El research #17 confirmó que SitioSimple merece entrar en la shortlist. La prueba práctica comparable de las tres finalistas continúa en #19.

SitioSimple combina costo fijo muy bajo, funciones locales para Argentina, administración no-code y capacidades interesantes para un futuro servicio administrado por Camila. Su principal riesgo es que parte del flujo operativo dependa de cuentas externas de pago/logística y termine más fragmentado que Tiendanube.

## Precio y prueba

Oferta publicada para Argentina:

- prueba completa: **15 días gratis**, sin tarjeta según la página comercial;
- Página Web + Tienda: **$3.900 ARS/mes equivalentes** contratando anual;
- total anual publicado: **$46.800 ARS**, IVA incluido;
- DonWeb no cobra comisión sobre ventas; el proveedor de pago sí puede cobrar su propia comisión.

El precio debe verificarse otra vez al momento de contratar/renovar porque DonWeb puede ofrecer condiciones diferentes según plazo.

Fuente:
- https://donweb.com/es-ar/crear-tienda-online

## Dominio, hosting y correo

El plan de tienda incluye:

- hosting;
- SSL;
- cuentas de correo;
- subdominio `*.misitiosimple.com`;
- en contratación anual, registro sin cargo durante el primer año de determinadas extensiones: `.online`, `.site`, `.website`, `.store` o `.uno` (excepto dominios premium).

Un `.com` o `.com.ar` no debe considerarse incluido: se puede contratar aparte o conectar uno existente.

Fuente:
- https://soporte.donweb.com/hc/es/articles/18691183839380-Conectar-mi-dominio-en-SitioSimple

## Catálogo y operación

La oferta/documentación pública incluye:

- catálogo de productos;
- gestión de stock, clientes y pedidos;
- promociones y cupones;
- actualización de precios con Excel;
- blog;
- editor drag-and-drop;
- soporte 24/7.

La profundidad exacta de variantes talle/color, stock por combinación, SKU por variante y exportación/importación completa del catálogo se verificará en #19 sobre la versión actual.

Fuente:
- https://donweb.com/es-ar/crear-tienda-online

## Pagos

Métodos documentados para Tienda Online:

- Mercado Pago;
- Mobbex;
- PayPal;
- transferencia/depósito;
- pago en entrega;
- a convenir;
- método propio.

Mercado Pago requiere conectar una cuenta del comercio y configurar sus credenciales en SitioSimple. El checkout documentado deriva al comprador a Mercado Pago y luego vuelve a la tienda.

Esto da libertad, pero la prueba debe medir:

- actualización automática del estado de orden;
- conciliación;
- cancelación/reintegro;
- si el reintegro se realiza en Mercado Pago y luego requiere reflejo manual en SitioSimple;
- cantidad de paneles que Camila debe usar por venta.

Fuentes:
- https://soporte.donweb.com/hc/es/articles/18546609299476-M%C3%A9todos-de-pago-disponibles-en-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18546251783444-Configurar-pago-con-Mercado-Pago

## Envíos

Métodos documentados:

- Andreani;
- OCA;
- Envia.com;
- retiro en local;
- a convenir;
- método propio.

Con Andreani y OCA se puede conectar una cuenta existente del operador. SitioSimple cotiza el envío y agrega su importe a la orden.

Con Envia.com, SitioSimple configura tarifas/opciones para checkout, pero la **gestión y realización efectiva de los envíos ocurre en la cuenta de Envia.com**. Puede ofrecer operadores como OCA, Andreani, Correo Argentino, FedEx y DHL según configuración.

Esta flexibilidad confirma a la vez el principal riesgo operativo: más paneles externos.

Fuentes:
- https://soporte.donweb.com/hc/es/articles/18547495468436-M%C3%A9todos-de-env%C3%ADo-disponibles-en-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18577117357844-Configurar-env%C3%ADo-con-Andreani
- https://soporte.donweb.com/hc/es/articles/18574569952404-Configurar-env%C3%ADo-con-OCA
- https://soporte.donweb.com/hc/es/articles/18580260215828-Configurar-Envia-com

## Pedidos y clientes

El panel de SitioSimple documenta una lista de ventas donde se puede:

- ver número de orden y comprador;
- consultar productos;
- modificar el estado de la venta;
- verificar el método de pago;
- conocer la situación del envío;
- ver datos de facturación;
- descargar una factura PDF generada por SitioSimple.

También se puede consultar una ficha del cliente y su historial de compras.

Esto alcanza para una pre-validación positiva de gestión básica. #19 debe verificar la trazabilidad real de cancelaciones/reintegros y del flujo de despacho.

Fuentes:
- https://soporte.donweb.com/hc/es/articles/18571940356884-Administrar-ventas-en-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18548443651860-Ver-datos-de-clientes-en-Sitio-Simple

## SEO, marketing y medición

SitioSimple publica/documenta:

- títulos, descripciones y URLs amigables;
- Google Shopping;
- Facebook Pixel;
- blog;
- integración con redes sociales;
- Email Marketing;
- estadísticas propias de ventas, visitas, fuentes de tráfico, navegadores y ubicación geográfica.

Para nuestro caso no alcanza con un dashboard: #19 debe verificar UTMs y medición de compra/revenue por fuente/campaña según `measurement.md`.

Como en las otras plataformas, estas herramientas técnicas no sustituyen el procedimiento editorial de `../playbook/04-seo-y-publicacion.md`.

Fuentes:
- https://donweb.com/es-ar/crear-sitio-web
- https://soporte.donweb.com/hc/es/articles/18539242603796-Estad%C3%ADsticas-de-mi-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18541389710356-Integraciones-en-SitioSimple

## Usuarios y permisos

Este punto es una fortaleza para nuestro modelo operativo.

La versión actual de SitioSimple permite:

- crear usuarios separados;
- seleccionar las secciones a las que cada usuario tiene acceso;
- activar/desactivar usuarios;
- modificar permisos;
- previsualizar qué ve ese usuario.

Esto encaja con la propuesta de que:

- el comercio sea propietario de cuentas/cobros;
- Camila tenga su propio acceso para operar;
- no se compartan contraseñas.

Fuente:
- https://soporte.donweb.com/hc/es/articles/36816025831060-C%C3%B3mo-acceder-al-editor-de-SitioSimple-y-gestionar-usuarios-y-permisos

## Servicio para múltiples comercios

DonWeb ofrece explícitamente SitioSimple para revendedores:

- administración de clientes/sitios;
- gestión de accesos y permisos;
- marca blanca;
- posibilidad de entregar acceso autoadministrable al cliente;
- un plan por cada sitio.

Esto **no forma parte del MVP** y no cambia la regla de que la tienda/cobros del comercio deben pertenecer al comercio. Sí es una ruta potencial si el servicio se replica luego.

Fuente:
- https://mailings.donweb.com/es-ar/revende-sitios-web

## Ventajas frente a Tiendanube Inicial

Documentalmente:

- permisos diferenciados;
- más opciones de pago;
- más opciones de envío;
- dominio propio disponible sin saltar a Tiendanube Esencial;
- algunas funciones masivas/Excel;
- correo/hosting incluidos;
- modelo revendedor futuro.

## Riesgos frente a Tiendanube Inicial

- costo fijo, aunque bajo;
- Mercado Pago ocurre mediante redirección y cuenta externa;
- Andreani/OCA pueden requerir cuentas externas;
- Envia.com exige gestionar el envío desde otro panel;
- más flexibilidad puede significar más configuración y procedimientos;
- todavía debemos verificar variantes, reembolsos, eventos de e-commerce, portabilidad y checkout móvil en el trial.

## Próximo paso

Ejecutar #19 usando [`protocolo-prueba-plataformas.md`](protocolo-prueba-plataformas.md). Este documento ya no tiene una decisión pendiente propia: DonWeb permanece en la shortlist hasta que la prueba práctica muestre una restricción concreta.
