# Shortlist de plataformas para el MVP

_Estado: shortlist acordada para evaluación. No es todavía la decisión final de plataforma._

## Plataformas activas

A partir de esta etapa, la evaluación práctica se concentra en tres opciones:

1. **Tiendanube**
2. **Empretienda**
3. **DonWeb SitioSimple**

Shopify, Wix, Odoo y otras alternativas quedan fuera de la evaluación activa salvo que aparezca una restricción nueva que invalide las tres opciones anteriores.

## Objetivo de la comparación

Elegir la plataforma más simple para que Camila pueda levantar y administrar la tienda online con baja carga operativa, buen encaje con Argentina y costo fijo razonable.

La comparación no debe premiar cantidad de funciones. Debe premiar la menor complejidad suficiente para operar correctamente.

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
- comportamiento con stock bajo/agota­do;
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

Usar el procedimiento de `docs/playbook/04-seo-y-publicacion.md` para comprobar:

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

Cuando sea posible usar trial/free tier, crear la misma mini tienda de prueba en las tres plataformas con:

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
9. revisión de métricas disponibles.

## Resultado esperado

La decisión final debe poder expresarse como:

> Elegimos **X** para el MVP porque cubre las operaciones reales de Camila con la menor complejidad y costo total razonables. Descartamos **Y** y **Z** por restricciones concretas verificadas.

La selección final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.
