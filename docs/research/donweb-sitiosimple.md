# DonWeb SitioSimple — evaluación para el MVP

[← Volver al índice de investigación](README.md) · [Comparar finalistas](shortlist-plataformas.md) · [Índice general](../INDEX.md)

_Verificado: 2026-09-16._

## Estado

**Candidato activo, no decisión final.**

SitioSimple entró en la shortlist porque combina costo fijo muy bajo, funciones locales para Argentina, administración no-code y capacidades interesantes para un futuro servicio administrado por Camila.

La prueba práctica del panel/checkout sigue pendiente en el issue #17.

## Precio y prueba

Oferta publicada para Argentina:

- prueba completa: **15 días gratis**, sin tarjeta;
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
- https://donweb.com/es-ar/crear-sitio-web

## Catálogo y operación

La oferta/documentación pública incluye:

- catálogo de productos;
- gestión de stock, clientes y pedidos;
- promociones y cupones;
- importación/carga masiva;
- edición de precios con Excel;
- blog;
- editor drag-and-drop;
- soporte 24/7.

Esto elimina varias restricciones presentes en Tiendanube Inicial, particularmente la falta de operaciones/carga masiva.

Fuentes:
- https://donweb.com/es-ar/crear-tienda-online
- https://soporte.donweb.com/hc/es/categories/18510452893844-SitioSimple

## Pagos

Métodos documentados para Tienda Online:

- Mercado Pago;
- Mobbex;
- PayPal;
- transferencia/depósito;
- pago en entrega;
- a convenir;
- método propio.

Mercado Pago requiere conectar una cuenta del comercio y configurar sus credenciales en SitioSimple. El checkout deriva al comprador a Mercado Pago y luego vuelve a la tienda.

Implicación operativa: hay más libertad que en Tiendanube Inicial, pero también más configuración de terceros y gestión de credenciales durante el alta.

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

Con Andreani y OCA se requiere cuenta con el operador. SitioSimple puede cotizar el envío y agregarlo a la orden.

Envia.com permite mostrar tarifas/opciones de múltiples operadores —incluyendo OCA, Andreani, Correo Argentino, FedEx y DHL según configuración— pero la gestión/realización del envío ocurre desde la cuenta de Envia.com.

Esto da más opciones logísticas que Tiendanube Inicial, a cambio de tener potencialmente una cuenta/panel externo adicional.

Fuentes:
- https://soporte.donweb.com/hc/es/articles/18547495468436-M%C3%A9todos-de-env%C3%ADo-disponibles-en-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18577117357844-Configurar-env%C3%ADo-con-Andreani
- https://soporte.donweb.com/hc/es/articles/18580260215828-Configurar-Envia-com

## SEO, marketing y medición

SitioSimple documenta:

- configuración de títulos, descripciones y URLs amigables;
- Google Shopping mediante feed;
- Facebook Pixel;
- blog;
- integración con redes sociales;
- Email Marketing incluido.

Como en las otras plataformas, esto resuelve herramientas técnicas pero no sustituye el procedimiento editorial de `../playbook/04-seo-y-publicacion.md`.

Fuentes:
- https://donweb.com/es-ar/crear-sitio-web
- https://soporte.donweb.com/hc/es/articles/23530424327956-Integrar-mi-tienda-con-Google-Shopping
- https://soporte.donweb.com/hc/es/articles/41953108813972-Configurar-Facebook-Pixel

## Usuarios y permisos

Este punto es una fortaleza para nuestro modelo operativo.

La versión actual de SitioSimple permite crear usuarios y seleccionar las secciones a las que cada usuario tendrá acceso. También permite activar/desactivar usuarios y modificar permisos.

A nivel de la cuenta DonWeb existe además gestión de usuarios/roles para colaborar sin compartir las credenciales del propietario.

Esto encaja con la propuesta de que:

- el comercio sea propietario de cuentas/cobros;
- Camila tenga su propio acceso para operar;
- no se compartan contraseñas.

Fuentes:
- https://soporte.donweb.com/hc/es/articles/36816025831060-C%C3%B3mo-acceder-al-editor-de-SitioSimple-y-gestionar-usuarios-y-permisos
- https://soporte.donweb.com/hc/es/articles/31678313142164-Gesti%C3%B3n-de-Usuarios

## Servicio para múltiples comercios

DonWeb ofrece explícitamente **SitioSimple Revendedores**:

- marca blanca;
- posibilidad de usar logo propio en el panel que ve el cliente;
- administración centralizada de sitios/clientes;
- accesos y permisos para clientes;
- un plan por cada sitio;
- DonWeb deja al revendedor definir su precio al cliente.

Esto **no forma parte del MVP de Camila** y no justifica construir un SaaS propio, pero reduce fricción si más adelante el mismo servicio se ofrece a otros comercios.

Fuentes:
- https://donweb.com/es-ar/revende-sitios-web
- https://donweb.com/es-ar/programa-de-partners

## Riesgos / puntos todavía no verificados

Antes de elegirlo hay que validar en la prueba:

1. experiencia real del panel para Camila;
2. variantes talle/color y actualización de stock;
3. flujo real pedido → pago → preparación → envío;
4. qué tan automática es la impresión/generación de etiquetas y seguimiento;
5. reintegros/cancelaciones desde la operación normal;
6. cobertura de seguro y logística inversa;
7. Google Analytics/eventos de e-commerce y calidad de la atribución;
8. exportación/portabilidad de productos, pedidos y clientes;
9. cumplimiento práctico del botón de arrepentimiento y páginas legales;
10. comportamiento del checkout en móvil.

## Condición para pasar a final

SitioSimple debería avanzar como candidato final si la prueba demuestra que un operador no técnico puede ejecutar el flujo completo sin depender regularmente de paneles externos o soporte y sin perder trazabilidad de pedidos/pagos/envíos.

Si el precio bajo se traduce en conciliación manual, saltos frecuentes entre sistemas o flujo de despacho débil, su ventaja económica pierde peso frente a Tiendanube.
