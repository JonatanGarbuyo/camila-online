# Shortlist de plataformas para el MVP

[← Índice de investigación](README.md) · [Índice general](../INDEX.md) · [Estado Wayfinder](../wayfinder/map.md)

_Estado: shortlist acordada para evaluación. No es todavía la decisión final de plataforma._

_Verificado documentalmente: 2026-09-16. La prueba práctica todavía está pendiente._

## Plataformas activas

A partir de esta etapa, la evaluación práctica se concentra exclusivamente en:

1. **Tiendanube**
2. **DonWeb SitioSimple**
3. **Empretienda**

Shopify, Wix, Odoo y otras alternativas quedan fuera de la evaluación activa salvo que aparezca una restricción nueva que invalide las tres opciones anteriores.

## Objetivo de la comparación

Elegir la plataforma más simple para que Camila pueda levantar y administrar la tienda online con baja carga operativa, buen encaje con Argentina y costo total razonable.

La comparación no debe premiar cantidad de funciones. Debe premiar la **menor complejidad suficiente para operar correctamente**.

## Matriz documental preliminar

Esta tabla sirve para orientar la prueba; no reemplaza probar los paneles con el caso real.

| Tema | Tiendanube Inicial | DonWeb SitioSimple Tienda | Empretienda |
| --- | --- | --- | --- |
| Costo fijo publicado | **$0** | **$3.900/mes equivalente** en contratación anual ($46.800/año) | **$10.490/mes** |
| Prueba | Plan gratis permanente | 15 días | 15 días según página comercial vigente |
| Comisión de plataforma | 0% usando Pago Nube | Sin comisión de DonWeb | Sin comisión de Empretienda |
| Pago principal | Pago Nube | Mercado Pago / Mobbex / transferencia / otros | Mercado Pago / Ualá Bis / transferencia / otros |
| Checkout/pago | Muy integrado al mismo administrador | Integra proveedores externos; Mercado Pago redirige y vuelve | Integra proveedores externos |
| Envíos | Andreani/Envío Nube | Andreani, OCA, Envia.com, retiro, propio | Andreani, OCA, Correo Argentino, E-Pick, retiro/personalizados |
| Dominio de entrada | `*.mitiendanube.com` | `*.misitiosimple.com` | `*.empretienda.com.ar` |
| Dominio propio | No en Inicial; requiere plan pago y dominio comprado aparte | Sí; anual incluye 1 año de extensiones seleccionadas, `.com/.com.ar` aparte | Sí; dominio se compra aparte |
| Carga/edición masiva | No en Inicial | Sí; carga/edición vía Excel documentada | Sí |
| Productos/ventas | Sin límites publicados | Catálogo/gestión incluidos | Ilimitados publicados |
| Usuarios/permisos | Usuarios ilimitados, **todos con acceso total** en Inicial | **Usuarios con permisos por secciones**; DonWeb también tiene roles de cuenta | **Pendiente de verificar**; documentación pública no confirma multiusuario seguro |
| SEO | Sitemap/Search Console, SEO de producto/categoría, Google Shopping | Titles/descripciones/URLs, Google Shopping, blog | SEO automático publicado, Google Shopping, blog; validar controles finos |
| Analítica | GA4 + Meta Pixel/CAPI | Pixel documentado; validar GA/e-commerce events en prueba | Google Analytics + Facebook Pixel publicados |
| Modelo multi-comercio futuro | Ecosistema de partners/apps, pero el plan Inicial no resuelve permisos granulares | **Revendedores/Partners, marca blanca y gestión de múltiples clientes** explícitos | Permite asesoramiento, pero no se verificó modelo multiusuario/revendedor equivalente |
| Principal ventaja | Cero costo fijo + flujo local integrado | Bajo costo + flexibilidad + permisos + modelo para administrar clientes | Simplicidad + muchas funciones locales en un único plan |
| Principal riesgo | Restricciones del plan $0 pueden generar trabajo manual o forzar upgrade caro | Más cuentas/proveedores externos pueden fragmentar operación | Accesos/permisos y profundidad de algunas integraciones todavía poco documentados públicamente |

### Fuentes principales

Tiendanube:
- https://www.tiendanube.com/planes-y-precios
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube
- https://ayuda.tiendanube.com/es_AR/pago-nube/que-es-pago-nube

DonWeb:
- [`donweb-sitiosimple.md`](donweb-sitiosimple.md)
- https://donweb.com/es-ar/crear-tienda-online
- https://soporte.donweb.com/hc/es/categories/18510452893844-SitioSimple

Empretienda:
- https://api.empretienda.com/

## Lectura actual de cada finalista

### Tiendanube

Es la referencia a superar por el **plan Inicial de costo fijo $0** y por tener pago y logística integrados en un mismo ecosistema.

Pago Nube tiene una ventaja operativa importante: centraliza pagos, devoluciones, contracargos y reportes dentro del administrador, y la transferencia tiene conciliación automática.

El costo de esa simplicidad es la rigidez del Inicial:

- solo Pago Nube como pago integrado;
- solo Andreani/Envío Nube;
- sin dominio propio;
- sin importación/exportación masiva de productos;
- sin exportación de ventas/clientes;
- sin acciones masivas;
- administradores con acceso total.

Si estas restricciones no molestan al volumen inicial, sigue siendo una opción muy fuerte.

### DonWeb SitioSimple

La investigación detallada está en [`donweb-sitiosimple.md`](donweb-sitiosimple.md).

Sobre documentación pública, ofrece mucho por un costo bajo:

- varios pagos y envíos locales;
- carga/edición masiva;
- dominio propio;
- SEO;
- usuarios con permisos diferenciados;
- soporte 24/7;
- posibilidad futura de Revendedores/Partners, marca blanca y administración de clientes.

Para el modelo futuro de Camila administrando tiendas ajenas, **permisos y modalidad revendedor son ventajas estructurales**.

La duda principal no es funcional sino operativa: Mercado Pago, Andreani/OCA o Envia.com pueden exigir cuentas/configuración externas. Hay que comprobar si el día a día queda suficientemente centralizado o si el ahorro mensual se paga con más pasos manuales.

### Empretienda

Es la alternativa más simple conceptualmente: un único plan de bajo costo con muchas funciones locales incluidas.

Publica:

- Mercado Pago y Ualá Bis;
- transferencia/efectivo;
- OCA, Correo Argentino, Andreani, E-Pick y envíos personalizados;
- importación masiva;
- productos/ventas ilimitados;
- dominio propio;
- Google Analytics;
- Facebook Pixel;
- Google Shopping;
- blog;
- SEO automático.

**Punto a verificar antes de considerarla apta para nuestro modelo:** la documentación pública consultada no confirma una gestión de usuarios/permisos equivalente a DonWeb. Los términos describen la cuenta/contraseña como personal e intransferible, por lo que no debemos diseñar una operación donde Camila y el comercio compartan una contraseña. Esto debe probarse o consultarse formalmente.

## Condiciones de descarte / cambio de plan

No queremos elegir por sensación. Estas condiciones permiten tomar decisiones concretas.

### Tiendanube Inicial deja de ser suficiente si…

- el catálogo real hace inviable cargar/editar productos uno por uno;
- se necesita dominio propio desde el lanzamiento;
- Pago Nube no puede habilitarse o no satisface la operación real;
- Andreani no sirve desde el origen/logística del comercio;
- se necesitan exportaciones/acciones masivas con frecuencia;
- los dueños no aceptan que Camila tenga acceso total al administrador;
- el costo de subir a Esencial/Impulso hace que otra finalista dé mejor operación a menor costo total.

Estas condiciones pueden descartar **el plan Inicial** sin necesariamente descartar Tiendanube como plataforma.

### DonWeb deja de ser suficiente si…

- el panel resulta confuso para Camila;
- el flujo normal obliga a alternar continuamente entre DonWeb, Mercado Pago y plataformas logísticas;
- no existe una operación suficientemente simple de etiquetas, seguimiento, cancelación y reintegro;
- medición/atribución de e-commerce es insuficiente para los KPIs acordados;
- faltan funciones críticas de cambios/devoluciones o cumplimiento que obliguen a demasiada operación manual;
- la prueba móvil del checkout muestra fricción material.

### Empretienda deja de ser suficiente si…

- no permite accesos separados y seguros para comercio + Camila;
- su operación obliga a compartir contraseña;
- el SEO configurable no alcanza el procedimiento del playbook;
- la integración de pagos/envíos requiere más operación manual de la esperada;
- portabilidad/exportación/reporting no resultan suficientes;
- el panel no escala razonablemente al catálogo/volumen real.

## Criterios de decisión

### 1. Operación no técnica

Validar que Camila pueda, sin desarrollo:

- crear y editar productos;
- administrar talles, colores y variantes;
- actualizar stock y precios;
- revisar pedidos;
- gestionar pagos/reintegros;
- preparar envíos;
- consultar clientes y estado de pedidos;
- modificar contenido/SEO;
- usar WhatsApp como canal de atención.

### 2. Catálogo y stock

Comparar:

- facilidad de alta manual;
- variantes por producto;
- comportamiento con stock bajo/agotado;
- carga/importación masiva si fuera necesaria;
- riesgo de desincronización con el local físico.

### 3. Pagos

Validar:

- medios de pago disponibles en Argentina;
- costo efectivo por venta;
- plazo de acreditación;
- reintegros;
- conciliación;
- dependencia de un único proveedor.

### 4. Envíos

Validar:

- Andreani y otras alternativas disponibles;
- generación de etiquetas;
- seguimiento;
- seguro;
- retiro en sucursal/punto;
- qué parte del flujo de cambios/devoluciones debe resolverse manualmente.

### 5. SEO y publicación

Usar [`../playbook/04-seo-y-publicacion.md`](../playbook/04-seo-y-publicacion.md) para comprobar:

- título SEO;
- meta description;
- URL editable;
- categorías;
- sitemap/indexación;
- imágenes y texto alternativo;
- páginas informativas;
- Google Shopping cuando aplique.

### 6. Analítica y atribución

Validar:

- Google Analytics;
- Meta Pixel / CAPI cuando corresponda;
- UTMs;
- medición de ventas y revenue;
- exportación/reporting suficiente para el MVP.

### 7. Titularidad y accesos

Validar:

- que tienda, cobros y facturación puedan quedar a nombre del comercio;
- que Camila pueda administrar la operación sin compartir credenciales personales;
- permisos disponibles para usuarios/administradores.

### 8. Costos

Comparar por separado:

- costo fijo mensual/anual;
- comisiones de plataforma;
- comisión del medio de pago;
- costo de envíos/seguro;
- dominio propio;
- aplicaciones o extras necesarios;
- costo operativo manual.

El costo fijo más bajo no gana automáticamente si genera más trabajo manual o errores.

## Prueba práctica propuesta

Crear la misma mini tienda de prueba en las tres plataformas cuando el trial/free tier lo permita, con:

- 3 a 5 productos ficticios;
- al menos un producto con talle y color;
- stock limitado;
- una categoría;
- una página informativa;
- configuración de SEO según el playbook;
- WhatsApp;
- un método de pago;
- un método de envío;
- Analytics/Pixel si el trial lo permite.

Luego ejecutar el mismo recorrido:

1. alta de producto;
2. actualización de precio/stock;
3. compra de prueba hasta donde la plataforma permita sin generar cargos innecesarios;
4. revisión del pedido en administración;
5. preparación del envío;
6. simulación de cancelación/reintegro;
7. búsqueda del producto desde el storefront;
8. edición SEO;
9. revisión de métricas disponibles;
10. creación de un acceso separado para el operador, si existe.

## Resultado esperado

La decisión final debe poder expresarse como:

> Elegimos **X** para el MVP porque cubre las operaciones reales de Camila con la menor complejidad y costo total razonables. Descartamos **Y** y **Z** por restricciones concretas verificadas.

La selección final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.
