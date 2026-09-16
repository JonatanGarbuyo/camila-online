# WhatsApp Business y canales sociales

_Verificado: 2026-09-16._

## Requisito: chat humano por WhatsApp

Tiendanube ofrece un botón nativo de WhatsApp configurable desde el administrador. El botón abre WhatsApp/WhatsApp Web y permite derivar consultas a un número del negocio sin necesidad de bot, API ni desarrollo.

Fuente:
- https://ayuda.tiendanube.com/es_AR/123362-whatsapp/como-deshabilitar-el-boton-de-whatsapp-en-mi-tiendanube
- https://ayuda.tiendanube.com/es_MX/como-agregar-el-boton-de-whatsapp-en-mi-tiendanube

> La documentación consultada para la activación está publicada bajo otra región, pero describe la funcionalidad nativa; la ayuda argentina confirma que el botón existe y se configura desde `Configuración > Botón de WhatsApp`.

## Nice-to-have: catálogo de WhatsApp

WhatsApp Business permite mantener un catálogo de productos y organizarlos en colecciones.

Además, Tiendanube publicó el 10/09/2026 un flujo para **conectar el catálogo de productos con WhatsApp Business a través de Meta Business Suite**. La sincronización se realiza desde la app de WhatsApp Business y requiere que el catálogo exista en Meta Business Suite.

Fuentes:
- https://faq.whatsapp.com/833697274483076/?cms_platform=web&locale=es_LA
- https://faq.whatsapp.com/2929318000711140/?cms_platform=web&locale=es_ES
- https://ayuda.tiendanube.com/es_AR/whatsapp/como-conectar-tu-catalogo-de-productos-con-whatsapp-business

### Implicación

El catálogo de WhatsApp es viable como canal de descubrimiento/asistencia sin convertir WhatsApp en el checkout principal. El camino recomendado sigue siendo:

`producto visto en WhatsApp/redes → tienda online → checkout integrado`

Esto preserva mejor stock, pago, envío y atribución.

## Facebook e Instagram

Meta Shopping / Facebook Shop / Instagram Shopping **no están disponibles en Argentina** desde el 10/08/2023 según la documentación vigente de Tiendanube.

Sin embargo, Tiendanube sí permite vincular la tienda con Meta Business Manager para sincronizar catálogo y utilizar otras capacidades como campañas/publicidad.

Fuentes:
- https://ayuda.tiendanube.com/es_AR/como-activar-instagram-shopping-en-mi-tiendanube
- https://ayuda.tiendanube.com/es_AR/como-activar-facebook-e-instagram-shopping

### Implicación

No diseñar el MVP suponiendo que habrá una tienda nativa dentro de Instagram/Facebook en Argentina. Esos canales deben funcionar principalmente como **adquisición y contenido**, enviando tráfico a la tienda online mediante links medibles.

## Medición

Mantener la regla definida en `docs/research/measurement.md`:

- todos los links desde Instagram/Facebook/WhatsApp deben llevar UTM cuando sea posible;
- Meta Pixel/CAPI se usa para conversiones en la tienda;
- las ventas que se cierren manualmente por WhatsApp pueden perder atribución automática y deben tratarse como excepción.

## Propuesta para el MVP

1. Usar **WhatsApp Business** con atención humana.
2. Activar el botón nativo de WhatsApp en la tienda.
3. Mantener checkout y pago en la tienda, no en chat.
4. Conectar catálogo de WhatsApp vía Meta Business Suite si el setup resulta simple y estable.
5. Usar Instagram/Facebook como fuentes de tráfico, no como storefront nativo en Argentina.

No se necesita WhatsApp Cloud API, bot ni agente automático en la primera etapa.