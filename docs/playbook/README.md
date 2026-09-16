# Playbook operativo — tienda online

Este directorio contendrá el manual durable para **levantar, lanzar y administrar** una tienda online usando la arquitectura finalmente aprobada.

El playbook es conocimiento reusable del servicio. Debe poder ser seguido por Camila u otro operador no técnico sin depender de chats anteriores.

## Estado

**Borrador de estructura.** La versión operativa debe completarse después de aprobar la plataforma en #9 y validar la operación real (#6, #7, #8, #13).

## Estructura prevista

1. `01-alta-y-titularidad.md`
   - quién crea y posee cada cuenta;
   - usuarios y permisos;
   - qué datos nunca compartir por chat/repo.

2. `02-configuracion-inicial.md`
   - identidad de marca;
   - plantilla/diseño;
   - datos legales y de contacto;
   - subdominio inicial y criterio para dominio propio.

3. `03-catalogo-y-stock.md`
   - alta de productos;
   - fotos;
   - talles/colores/variantes;
   - SKU;
   - stock y reconciliación con local físico.

4. `04-seo-y-publicacion.md`
   - títulos, descripciones, categorías y URLs;
   - SEO title/meta description;
   - imágenes y texto alternativo;
   - Search Console/sitemap;
   - Google Shopping;
   - checklist antes de publicar un producto.

5. `05-pagos.md`
   - alta/configuración sin guardar credenciales;
   - medios de pago;
   - plazo de acreditación;
   - conciliación y reintegros.

6. `06-envios.md`
   - configuración logística;
   - pesos/dimensiones;
   - etiquetas;
   - seguro;
   - despacho y seguimiento.

7. `07-cambios-devoluciones.md`
   - arrepentimiento legal;
   - cambios de talle;
   - devolución y reintegro;
   - logística inversa.

8. `08-whatsapp-y-atencion.md`
   - WhatsApp Business;
   - horarios/responsabilidad;
   - respuestas frecuentes;
   - escalamiento de incidencias.

9. `09-redes-y-adquisicion.md`
   - Instagram/Facebook;
   - UTMs;
   - links de bio/story/post/referidos;
   - recomendaciones de publicación.

10. `10-medicion-y-reporte.md`
    - GA4;
    - Meta Pixel/CAPI;
    - KPIs semanales;
    - atribución y ventas asistidas.

11. `11-operacion-diaria.md`
    - checklist diario/semanal;
    - pedidos pendientes;
    - stock/precio;
    - mensajes;
    - despachos;
    - reclamos y devoluciones.

12. `12-lanzamiento.md`
    - checklist técnico/operativo/legal;
    - compra de prueba;
    - pago de prueba;
    - envío de prueba;
    - verificación SEO/analytics;
    - go/no-go.

## Regla editorial

El playbook debe explicar **qué hacer y cómo verificar que quedó bien**. No debe contener contraseñas, tokens, API keys, CUIT de clientes, datos de tarjetas ni credenciales.

Cuando un procedimiento cambie por actualización de un proveedor, actualizar el playbook y registrar fecha/fuente cuando la diferencia sea material.