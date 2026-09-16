# Plataformas: free tiers, precios y SEO

_Verificado: 2026-09-16._

Este documento compara alternativas no-code relevantes para el MVP. No constituye una decisión final de plataforma; esa decisión vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.

## Tiendanube Argentina

### Planes actuales

- Inicial: **$0 ARS/mes**.
- Esencial: **$26.999 ARS/mes**.
- Impulso: **$78.999 ARS/mes**.
- Escala: **$234.999 ARS/mes**.
- Evolución: precio a consultar.

El plan Inicial es permanente y no solo una prueba. Incluye productos/ventas/visitas sin límite indicado, Pago Nube, Andreani, GA4, WhatsApp, Google Shopping y Meta Pixel/CAPI. No permite dominio propio, importación/exportación masiva, exportación de ventas/clientes, permisos diferenciados, otros medios de pago/envío ni GTM.

Dominio propio: nice-to-have; requiere pasar a un plan pago.

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

## Odoo Online

- Plan **One App Free: US$0**, una aplicación con usuarios ilimitados y hosting Odoo Online.
- Si la app elegida depende de otras aplicaciones —por ejemplo eCommerce depende de Website e Invoicing— Odoo indica que las dependencias necesarias también se incluyen gratis.

### SEO

Odoo tiene una capa SEO técnica completa: edición de metadatos, sitemap automático, robots.txt, datos estructurados/schema.org y herramientas de optimización de contenido.

### Encaje

Es una alternativa gratuita real y técnicamente potente, pero no es actualmente la baseline: para Argentina puede requerir más configuración de pagos, logística y operación que una plataforma local-first. Evaluar solo si Tiendanube/Empretienda quedan bloqueadas por una restricción concreta.

Fuentes:
- https://www.odoo.com/pricing
- https://www.odoo.com/documentation/19.0/applications/websites/website/structure/seo.html

## Shopify Argentina

- Prueba: **3 días gratis**.
- Promoción vigente consultada: **US$1/mes durante 3 meses** después de la prueba.
- Basic: **US$19/mes pagando anual** o **US$25/mes pagando mensual**.
- No tiene capa permanente gratuita para operar una tienda.

Shopify incluye SEO técnico base (estructura de URL, jerarquía, sitemap, etc.) y permite optimizaciones editoriales, pero agrega costo fijo en USD y no es local-first para este MVP.

Fuentes:
- https://www.shopify.com/ar/precios
- https://help.shopify.com/es/manual/promoting-marketing/seo/optimize-site

## Wix

- Permite crear/publicar un sitio gratuito, pero **para aceptar pagos hay que hacer upgrade a un plan que admita pagos**.
- Mercado Pago está soportado en Argentina.
- Los precios de planes pagos son localizados/dinámicos; verificar el valor final en la cuenta antes de comparar costo.

Wix tiene una capa SEO fuerte: sitemap automático, SEO para productos/categorías y datos estructurados predeterminados en Wix Stores. No es un free tier de e-commerce transaccional para nuestro requisito.

Fuentes:
- https://support.wix.com/es/article/elegir-un-plan-premium
- https://support.wix.com/es/article/conectar-mercado-pago-como-proveedor-de-pagos
- https://support.wix.com/es/article/wix-stores-seo-para-las-p%C3%A1ginas-de-productos
- https://support.wix.com/es/article/entender-el-archivo-del-sitemap-de-tu-sitio

## Ecwid

Ecwid actualmente documenta cuatro **planes pagos**: Starter, Venture, Business y Unlimited. Starter permite hasta 10 productos y vender, pero no debe tratarse como un plan gratuito permanente. La página pública no expuso el precio localizado en la consulta, por lo que debe verificarse desde facturación antes de usarlo en una comparación económica.

Ecwid ofrece SEO técnico, pero varias capacidades avanzadas —incluido sitemap para Instant Site según su ayuda actual— están disponibles desde Venture en adelante.

Fuentes:
- https://support.ecwid.com/hc/es/articles/207100729-Planes-y-caracter%C3%ADsticas-de-Ecwid
- https://support.ecwid.com/hc/es/articles/360000585949-Qu%C3%A9-hace-Ecwid-por-el-SEO

## Conclusión provisional

Para este MVP argentino no-code y de costo fijo mínimo:

1. **Tiendanube Inicial** sigue siendo la baseline por ser $0 permanente y tener pagos/logística/medición locales integrados.
2. **Empretienda** es un fallback especialmente interesante si pagar $10.490/mes simplifica dominio, medios de pago/envío, carga masiva o administración.
3. **Odoo One App Free** queda como alternativa secundaria gratuita, con mayor riesgo de complejidad operativa/local.
4. Wix, Shopify y Ecwid no ofrecen hoy una capa gratuita permanente que cumpla el checkout online del MVP sin pasar a un plan pago.

La selección final sigue bloqueada por la operación real de Camila, catálogo/stock, cambios/devoluciones y esquema de accesos/titularidad.