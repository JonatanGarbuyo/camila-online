# Plataformas: free tiers, precios y SEO

_Verificado: 2026-09-16._

Este documento conserva la investigación amplia de alternativas no-code relevantes para el MVP. La evaluación activa quedó reducida a **Tiendanube, Empretienda y DonWeb SitioSimple**. La decisión final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.

## Shortlist activa

- **Tiendanube** — baseline por costo fijo $0 en el plan Inicial y buen fit local.
- **Empretienda** — alternativa local simple de precio fijo bajo.
- **DonWeb SitioSimple** — alternativa local de costo muy bajo que requiere validación práctica.

La metodología de comparación práctica está en `docs/research/shortlist-plataformas.md`.

Shopify, Wix, Odoo y otras alternativas quedan fuera de la evaluación activa salvo que aparezca una restricción nueva que invalide las tres opciones anteriores.

## Tiendanube Argentina

### Planes actuales

- Inicial: **$0 ARS/mes**.
- Esencial: **$26.999 ARS/mes**.
- Impulso: **$78.999 ARS/mes**.
- Escala: **$234.999 ARS/mes**.
- Evolución: precio a consultar.

El plan Inicial es permanente y no solo una prueba. Incluye productos/ventas/visitas sin límite indicado, Pago Nube, Andreani, GA4, WhatsApp, Google Shopping y Meta Pixel/CAPI. No permite dominio propio, importación/exportación masiva, exportación de ventas/clientes, permisos diferenciados, otros medios de pago/envío ni GTM.

El plan Esencial habilita dominio propio, pero **el costo del dominio no está incluido**: debe comprarse y renovarse aparte.

Dominio propio: nice-to-have; no bloquea el MVP.

### SEO

Tiendanube resuelve una parte importante de SEO técnico y permite optimización manual:

- sitemap XML generado y actualizado automáticamente;
- verificación e integración con Google Search Console;
- título SEO, meta descripción y URL editable para productos y categorías;
- páginas de contenido con título/meta descripción;
- datos generales del negocio usados para SEO;
- texto alternativo en imágenes dentro de contenido y soporte de alt text en flujos de producto;
- integración con Google Shopping.

La plataforma no reemplaza el trabajo editorial: títulos, descripciones, categorías, fotografías, guía de talles, políticas y contenido original deben ser preparados por quien administra la tienda.

Fuentes:
- https://www.tiendanube.com/planes-y-precios
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube
- https://ayuda.tiendanube.com/160435-seo-del-producto/que-son-las-opciones-avanzadas-de-seo-de-mis-productos
- https://ayuda.tiendanube.com/es_AR/google/como-enviar-un-sitemap-a-google
- https://ayuda.tiendanube.com/es_AR/google/como-verificar-mi-tienda-con-google

## Empretienda

- Prueba: **15 días gratis**.
- Luego: **$10.490 ARS/mes finales**.
- Sin comisión de plataforma por venta.
- Un único plan.
- Incluye dominio gratuito `*.empretienda.com.ar` y permite conectar dominio propio sin costo adicional de plataforma.
- Incluye Mercado Pago, Ualá Bis, transferencia/efectivo; OCA, Correo Argentino, Andreani, E-Pick y métodos personalizados; carga masiva; GA; Facebook Pixel; Google Shopping; blog y productos/ventas ilimitados.

### SEO

Empretienda declara **optimización para SEO automática** e incluye blog, páginas informativas, Google Analytics y Google Shopping. La información pública consultada no documenta con el mismo nivel de detalle que Tiendanube las capacidades de meta tags, sitemap, redirects o datos estructurados; si Empretienda pasa a finalista, validar esas funciones en la prueba de 15 días.

Fuente primaria:
- https://api.empretienda.com/

## DonWeb SitioSimple

DonWeb publica SitioSimple como constructor de sitio + tienda online orientado al mercado argentino.

Oferta verificada durante esta investigación:

- prueba: **15 días**;
- precio promocionado equivalente: **$3.900 ARS/mes** contratando **$46.800 ARS anuales, IVA incluido**;
- sin comisión de plataforma por venta indicada en la oferta consultada;
- catálogo y stock;
- carga masiva;
- Mercado Pago, Mobbex y transferencia;
- Andreani, OCA y Envia.com;
- Google Shopping;
- Meta/Facebook Pixel;
- blog;
- campos SEO editables en productos/categorías;
- hosting y SSL.

### Dominio

El beneficio de dominio incluido en determinados planes/promociones debe leerse con precisión: la documentación consultada indica un dominio gratuito por un año para ciertas extensiones promocionales, por ejemplo `.site`, `.online`, `.store`, `.uno` y `.website`. No asumir que incluye un `.com.ar`.

### SEO

SitioSimple permite editar metadatos y URLs de contenido/productos, por lo que cubre la base del SEO on-page. Debe validarse en prueba real sitemap, indexación, datos estructurados y facilidad del flujo para operador no técnico.

Fuentes:
- https://donweb.com/es-ar/crear-tienda-online
- https://soporte.donweb.com/hc/es/articles/18573714829460-Posicionamiento-Web-de-mi-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18691183839380-Conectar-mi-dominio-en-SitioSimple

Research específico abierto: issue #17.

## Alternativas fuera de evaluación activa

Las siguientes plataformas fueron investigadas, pero quedan fuera de la shortlist actual.

### Odoo Online

- Plan **One App Free: US$0**, una aplicación con usuarios ilimitados y hosting Odoo Online.
- Si la app elegida depende de otras aplicaciones —por ejemplo eCommerce depende de Website e Invoicing— Odoo indica que las dependencias necesarias también se incluyen gratis.
- Capa SEO técnica potente.

Queda fuera de evaluación activa por complejidad para operadores no técnicos. Solo reconsiderar si las tres opciones locales quedan bloqueadas.

Fuentes:
- https://www.odoo.com/pricing
- https://www.odoo.com/documentation/19.0/applications/websites/website/structure/seo.html

### Shopify Argentina

- Prueba: **3 días gratis**.
- Promoción consultada: **US$1/mes durante 3 meses** después de la prueba.
- Basic: **US$19/mes pagando anual** o **US$25/mes pagando mensual**.
- No tiene capa permanente gratuita para operar una tienda.
- Funciona en Argentina y puede integrarse con Mercado Pago, pero agrega costo en USD y complejidad/comisiones asociadas a proveedores externos de pago.

Fuentes:
- https://www.shopify.com/ar/precios
- https://help.shopify.com/es/manual/promoting-marketing/seo/optimize-site

### Wix

- Permite crear/publicar un sitio gratuito, pero para aceptar pagos hay que hacer upgrade a un plan que admita pagos.
- Mercado Pago está soportado en Argentina.
- Buena capa SEO técnica.

Queda fuera de evaluación activa porque no aporta una ventaja decisiva frente a las opciones locales para este MVP.

Fuentes:
- https://support.wix.com/es/article/elegir-un-plan-premium
- https://support.wix.com/es/article/conectar-mercado-pago-como-proveedor-de-pagos
- https://support.wix.com/es/article/wix-stores-seo-para-las-p%C3%A1ginas-de-productos
- https://support.wix.com/es/article/entender-el-archivo-del-sitemap-de-tu-sitio

### Ecwid

Ecwid documenta planes pagos Starter, Venture, Business y Unlimited. Starter permite hasta 10 productos, pero no debe tratarse como plan gratuito permanente. Queda fuera de evaluación activa.

Fuentes:
- https://support.ecwid.com/hc/es/articles/207100729-Planes-y-caracter%C3%ADsticas-de-Ecwid
- https://support.ecwid.com/hc/es/articles/360000585949-Qu%C3%A9-hace-Ecwid-por-el-SEO

## Conclusión de investigación

La siguiente etapa ya no consiste en buscar más proveedores. Consiste en validar la shortlist de tres contra la operación real del negocio y el mismo escenario de prueba:

1. **Tiendanube**
2. **Empretienda**
3. **DonWeb SitioSimple**

La selección final sigue bloqueada por la operación real de Camila, catálogo/stock, cambios/devoluciones, esquema de accesos/titularidad y la prueba práctica de DonWeb.
