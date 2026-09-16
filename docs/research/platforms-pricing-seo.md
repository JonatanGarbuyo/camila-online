# Plataformas: free tiers, precios, Argentina y SEO

_Verificado: 2026-09-16._

Este documento compara alternativas no-code relevantes para el MVP. No constituye una decisión final de plataforma; esa decisión vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.

## Shortlist actual

1. **Tiendanube Inicial** — baseline por costo fijo $0 y muy buen fit local.
2. **DonWeb SitioSimple** — alternativa local de costo muy bajo que merece validación práctica.
3. **Empretienda** — alternativa local simple, de precio fijo bajo y sin comisión de plataforma.
4. **Shopify / Wix** — funcionan en Argentina, pero son plataformas globales menos local-first y con costo mayor o más complejidad local.
5. **Odoo Online** — última opción para este caso por complejidad operativa para usuarios no técnicos, aun cuando su free tier sea potente.

## Tiendanube Argentina

### Planes actuales

- Inicial: **$0 ARS/mes**.
- Esencial: **$26.999 ARS/mes**.
- Impulso: **$78.999 ARS/mes**.
- Escala: **$234.999 ARS/mes**.
- Evolución: precio a consultar.

El plan Inicial es permanente y no solo una prueba. Incluye productos/ventas/visitas sin límite indicado, Pago Nube, Andreani, GA4, WhatsApp, Google Shopping y Meta Pixel/CAPI. No permite dominio propio, importación/exportación masiva, exportación de ventas/clientes, permisos diferenciados, otros medios de pago/envío ni GTM.

### Dominio propio

**El plan Esencial no incluye el costo del dominio.** El plan pago habilita a conectar un dominio propio, pero el dominio se compra/renueva aparte.

Tiendanube permite comprar un `.com` desde su administrador o conectar uno comprado en un proveedor externo. El plan Inicial no permite dominio propio.

Para el MVP, dominio propio sigue siendo **nice-to-have** y no bloquea el lanzamiento.

### SEO

Tiendanube resuelve una parte importante de SEO técnico y permite optimización manual:

- sitemap XML generado y actualizado automáticamente;
- verificación e integración con Google Search Console;
- título SEO, meta descripción y URL editable para productos y categorías;
- páginas de contenido con título/meta descripción;
- datos generales del negocio usados para SEO;
- soporte de contenido e imágenes optimizables;
- integración con Google Shopping.

La plataforma no reemplaza el trabajo editorial. El procedimiento reusable vive en `docs/playbook/04-seo-y-publicacion.md`.

Fuentes:
- https://www.tiendanube.com/planes-y-precios
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube
- https://ayuda.tiendanube.com/es_AR/como-conseguir-mi-dominio-propio
- https://ayuda.tiendanube.com/es_AR/175774-configuracion-del-dominio-propio/como-usar-mi-dominio-propio-en-mi-tienda
- https://ayuda.tiendanube.com/160435-seo-del-producto/que-son-las-opciones-avanzadas-de-seo-de-mis-productos
- https://ayuda.tiendanube.com/es_AR/google/como-enviar-un-sitemap-a-google

## DonWeb SitioSimple

### Precio y prueba

La oferta pública argentina consultada muestra:

- **15 días de prueba gratis**, sin tarjeta;
- Página Web + Tienda: **$3.900 ARS/mes equivalente**, con total anual publicado de **$46.800 ARS**, IVA incluido;
- sin comisión de plataforma por venta.

El precio mostrado en la landing está asociado al total anual; DonWeb permite elegir plazo y publica descuentos mayores para períodos más largos. Confirmar precio final/renovación antes de contratar.

### Qué incluye relevante al MVP

- editor visual/IA, sin programación;
- catálogo, variantes y stock;
- carga masiva de productos / actualización por Excel;
- Mercado Pago, Mobbex, transferencia, PayPal y otras opciones;
- Andreani, OCA, Envia.com y métodos propios;
- Envia.com puede cotizar operadores como OCA, Andreani, Correo Argentino, FedEx y DHL;
- Google Shopping;
- Facebook Pixel;
- blog;
- soporte 24/7;
- SSL y hosting;
- campos SEO de producto y categoría;
- SEO por página: meta title, meta description y URL slug.

### Dominio

La publicidad dice “dominio gratis”, pero la ayuda vigente aclara el alcance: con plan anual se ofrece **1 dominio gratis por un año** en ciertas extensiones como `.site`, `.online`, `.store`, `.uno` o `.website`.

No asumir que incluye un `.com` o `.com.ar`. Puede conectarse un dominio comprado aparte.

### Evaluación provisional

DonWeb SitioSimple es **una alternativa seria** y entra a la shortlist. En costo fijo es muy competitivo y tiene integraciones argentinas suficientes sobre el papel.

Antes de desplazar a Tiendanube como baseline hay que validar en prueba real:

- facilidad de operación diaria para Camila;
- experiencia de checkout;
- flujo completo Pago/Envío;
- atribución/analytics;
- portabilidad/exportación de datos;
- cambios/reintegros;
- calidad de la administración de pedidos;
- condiciones reales de renovación/dominio.

Issue: #17.

Fuentes:
- https://donweb.com/es-ar/crear-tienda-online
- https://soporte.donweb.com/hc/es/categories/18510452893844-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18546251783444-Configurar-pago-con-Mercado-Pago
- https://soporte.donweb.com/hc/es/articles/34280035219988--C%C3%B3mo-migrar-mi-tienda-online-de-Mercado-Shops-a-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18580260215828-Configurar-Envia-com
- https://soporte.donweb.com/hc/es/articles/18573931290644-Agregar-productos-en-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18548878640276-Crear-categor%C3%ADas-de-producto-en-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18573714829460-Posicionamiento-Web-de-mi-SitioSimple
- https://soporte.donweb.com/hc/es/articles/18691183839380-Conectar-mi-dominio-en-SitioSimple

## Empretienda

### Encaje en Argentina

Empretienda es local-first y está orientada a administración no técnica.

- Prueba: **15 días gratis**.
- Luego: **$10.490 ARS/mes finales**.
- Sin comisión de plataforma por venta.
- Un único plan.
- Productos y ventas ilimitadas.
- Subdominio gratuito `*.empretienda.com.ar`.
- Permite conectar dominio propio; el dominio se compra aparte.
- Mercado Pago, Ualá Bis, transferencia/efectivo y otros flujos configurables.
- Integraciones de envío locales, entre ellas OCA, y la oferta pública lista integraciones de envío y métodos personalizados.
- GA, Facebook Pixel, Google Shopping, blog, WhatsApp y gestión de stock.

### SEO

Empretienda declara **optimización SEO automática**. La documentación pública consultada no explica con el mismo detalle que Tiendanube o DonWeb todas las capacidades técnicas; si queda finalista, validar en los 15 días de prueba:

- title/meta por producto y categoría;
- sitemap;
- redirects;
- canonical;
- datos estructurados;
- Search Console.

### Evaluación provisional

Muy buen fit para operador no técnico y comercio argentino. Su principal trade-off frente a Tiendanube es un ecosistema/integraciones menos amplio; frente a DonWeb, cuesta más por mes según precios publicados, aunque ofrece un producto e-commerce enfocado y simple.

Fuentes:
- https://api.empretienda.com/
- https://empretienda.helpjuice.com/es_AR/como-configurar-o-editar-tu-dominio-

## Shopify Argentina

### Alcance local

Shopify puede operar en Argentina y Mercado Pago tiene integración oficial para Shopify sin desarrollo.

Precios vigentes consultados:

- prueba **3 días gratis**;
- promoción: **US$1/mes durante 3 meses**;
- Basic: **US$19/mes** con pago anual o **US$25/mes** mensual;
- Grow: US$49/mes anual;
- Advanced: US$299/mes anual.

Cuando se usa un proveedor de pago externo, Shopify publica cargos adicionales de plataforma:

- Basic: **2%**;
- Grow: **1%**;
- Advanced: **0,6%**.

Esos cargos se suman a los costos propios del procesador de pagos.

Mercado Pago ofrece Checkout Pro y pagos con tarjeta integrados para Shopify en Argentina.

### Logística/fiscalidad

Shopify tiene un ecosistema amplio de apps y existe una app de Correo Argentino, pero no tiene la misma capa local integrada de punta a punta que Tiendanube/DonWeb/Empretienda.

La fiscalidad argentina no viene resuelta como un circuito ARCA nativo: Shopify documenta configuración de impuestos genérica y uso de terceros cuando corresponde.

### Evaluación provisional

Plataforma muy potente y madura, pero para este MVP agrega:

- costo en USD;
- comisión adicional con proveedor externo;
- más dependencia de apps para localización argentina.

No es primera opción mientras las plataformas locales cubran el caso.

Fuentes:
- https://www.shopify.com/ar/precios
- https://www.mercadopago.com.ar/developers/es/docs/shopify/overview
- https://help.shopify.com/es/manual/payments/third-party-providers
- https://help.shopify.com/es/manual/taxes

## Wix

### Alcance local

Wix permite construir un sitio gratis, pero **para aceptar pagos online hay que contratar un plan Premium que soporte pagos/e-commerce**.

En Argentina:

- Mercado Pago está soportado oficialmente;
- Wix Stores permite reglas de envío por regiones, entrega y retiro;
- el precio de los planes varía según ubicación/cuenta y debe verificarse en checkout;
- planes anuales elegibles pueden incluir un cupón de dominio por 1 año, pero dominio y plan son suscripciones separadas.

### SEO

Wix tiene una capa SEO fuerte: sitemap, configuración SEO, datos estructurados y herramientas para productos.

### Evaluación provisional

Funciona en Argentina y es muy bueno como constructor web/SEO, pero para este caso no tiene ventaja suficiente sobre plataformas locales:

- no hay checkout gratuito permanente;
- pagos locales sí, pero logística argentina es menos directa;
- pricing menos simple/local para comparar;
- el foco del proyecto es operación e-commerce simple, no diseño web generalista.

Fuentes:
- https://support.wix.com/es/article/elegir-un-plan-premium
- https://support.wix.com/es/article/conectar-mercado-pago-como-proveedor-de-pagos
- https://support.wix.com/es/article/wix-stores-crear-regiones-de-env%C3%ADo-y-entrega
- https://support.wix.com/es/article/comprar-un-dominio-frente-a-comprar-un-plan-premium

## Odoo Online

- Plan **One App Free: US$0**, una aplicación con usuarios ilimitados y hosting Odoo Online.
- Si eCommerce depende de Website/Invoicing, Odoo indica que las dependencias necesarias se incluyen gratis.
- Capa SEO técnica completa.

### Evaluación para este proyecto

Aunque es potente y puede ser barato, queda como **última alternativa** para el MVP. El riesgo principal no es técnico sino operativo: más conceptos/configuración para una administradora no técnica y menor localización argentina lista para usar.

Evaluar solo si las opciones locales quedan bloqueadas por una necesidad concreta.

Fuentes:
- https://www.odoo.com/pricing
- https://www.odoo.com/documentation/19.0/applications/websites/website/structure/seo.html

## Ecwid

Ecwid documenta planes pagos Starter, Venture, Business y Unlimited. No tratarlo como free tier permanente para el MVP actual. Tiene SEO técnico, pero no presenta una ventaja local clara frente a la shortlist.

Fuentes:
- https://support.ecwid.com/hc/es/articles/207100729-Planes-y-caracter%C3%ADsticas-de-Ecwid
- https://support.ecwid.com/hc/es/articles/360000585949-Qu%C3%A9-hace-Ecwid-por-el-SEO

## Conclusión provisional

La decisión final **no está tomada**.

La shortlist queda:

- **Tiendanube Inicial**: mejor baseline gratuita/local hasta ahora.
- **DonWeb SitioSimple**: challenger local de costo fijo muy bajo; necesita prueba práctica.
- **Empretienda**: opción local simple y predecible, especialmente si se prioriza facilidad operativa.

Shopify y Wix funcionan en Argentina pero hoy agregan costo/complejidad sin una ventaja decisiva para este MVP. Odoo queda como última opción por complejidad para usuarios no técnicos.

La selección final sigue bloqueada por operación real de Camila, catálogo/stock, cambios/devoluciones, accesos/titularidad y la validación de DonWeb (#17).