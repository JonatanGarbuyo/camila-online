# Playbook operativo — tienda online

[← Volver al índice general](../INDEX.md) · [Ver investigación](../research/README.md) · [Ver estado Wayfinder](../wayfinder/map.md)

Este directorio contendrá el manual durable para **levantar, lanzar y administrar** una tienda online usando la arquitectura finalmente aprobada.

El playbook es conocimiento reusable del servicio. Debe poder ser seguido por Camila u otro operador no técnico sin depender de chats anteriores.

## Estado

**Borrador de estructura.** La versión operativa debe completarse después de aprobar la plataforma en #9 y validar la operación real (#6, #7, #8, #13).

Leyenda:

- ✅ procedimiento usable;
- 📝 pendiente de completar;
- 🔒 depende de una decisión o información todavía abierta.

## Índice del playbook

1. 🔒 `01-alta-y-titularidad.md`
   - quién crea y posee cada cuenta;
   - usuarios y permisos;
   - qué datos nunca compartir por chat/repo.

2. 🔒 `02-configuracion-inicial.md`
   - identidad de marca;
   - plantilla/diseño;
   - datos legales y de contacto;
   - subdominio inicial y criterio para dominio propio.

3. 🔒 `03-catalogo-y-stock.md`
   - alta de productos;
   - fotos;
   - talles/colores/variantes;
   - SKU;
   - stock y reconciliación con local físico.

4. ✅ [`04-seo-y-publicacion.md`](04-seo-y-publicacion.md)
   - títulos, descripciones, categorías y URLs;
   - SEO title/meta description;
   - imágenes y texto alternativo;
   - Search Console/sitemap;
   - Google Shopping;
   - checklist antes de publicar un producto.

5. 📝 `05-pagos.md`
   - alta/configuración sin guardar credenciales;
   - medios de pago;
   - plazo de acreditación;
   - conciliación y reintegros.
   - investigación fuente: [`../research/payments.md`](../research/payments.md).

6. 📝 `06-envios.md`
   - configuración logística;
   - pesos/dimensiones;
   - etiquetas;
   - seguro;
   - despacho y seguimiento.
   - investigación fuente: [`../research/shipping-insurance.md`](../research/shipping-insurance.md).

7. 🔒 `07-cambios-devoluciones.md`
   - arrepentimiento legal;
   - cambios de talle;
   - devolución y reintegro;
   - logística inversa.
   - investigación legal: [`../research/legal-consumer.md`](../research/legal-consumer.md).

8. 📝 `08-whatsapp-y-atencion.md`
   - WhatsApp Business;
   - horarios/responsabilidad;
   - respuestas frecuentes;
   - escalamiento de incidencias.
   - investigación fuente: [`../research/social-whatsapp.md`](../research/social-whatsapp.md).

9. 📝 `09-redes-y-adquisicion.md`
   - Instagram/Facebook;
   - UTMs;
   - links de bio/story/post/referidos;
   - recomendaciones de publicación.

10. 📝 `10-medicion-y-reporte.md`
    - GA4;
    - Meta Pixel/CAPI;
    - KPIs semanales;
    - atribución y ventas asistidas.
    - investigación fuente: [`../research/measurement.md`](../research/measurement.md).

11. 🔒 `11-operacion-diaria.md`
    - checklist diario/semanal;
    - pedidos pendientes;
    - stock/precio;
    - mensajes;
    - despachos;
    - reclamos y devoluciones.

12. 🔒 `12-lanzamiento.md`
    - checklist técnico/operativo/legal;
    - compra de prueba;
    - pago de prueba;
    - envío de prueba;
    - verificación SEO/analytics;
    - go/no-go.

## Regla editorial

El playbook debe explicar **qué hacer y cómo verificar que quedó bien**. No debe contener contraseñas, tokens, API keys, CUIT de clientes, datos de tarjetas ni credenciales.

Cuando un procedimiento cambie por actualización de un proveedor, actualizar el playbook y registrar fecha/fuente cuando la diferencia sea material.

## SEO/publicación — criterios independientes de plataforma

El procedimiento usable ya vive en [`04-seo-y-publicacion.md`](04-seo-y-publicacion.md). En resumen, el playbook exige:

- nombres de producto entendibles por clientes, no códigos internos;
- descripciones originales con material, calce, medidas/talles, color, cuidados y atributos relevantes;
- categorías basadas en cómo busca la gente, no solo en organización interna;
- título SEO y meta descripción revisados antes de publicar;
- URL corta y descriptiva cuando la plataforma permita editarla;
- imágenes nítidas y texto alternativo descriptivo cuando esté disponible;
- guía de talles en texto/HTML además de imágenes cuando sea posible;
- páginas de contenido: quiénes somos, cómo comprar, envíos, cambios/devoluciones, preguntas frecuentes y contacto;
- Search Console + sitemap una vez pública la tienda;
- UTMs en links comerciales de Instagram/Facebook/WhatsApp/referrals;
- no copiar descripciones del proveedor o de otras tiendas;
- revisar que precio, stock, variantes, peso y dimensiones sean correctos antes de publicar.

El SEO técnico del proveedor ayuda, pero el contenido y la disciplina editorial siguen siendo responsabilidad del operador.
