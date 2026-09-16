# Protocolo de prueba — Tiendanube vs DonWeb vs Empretienda

_Estado: protocolo listo. La prueba práctica en paneles la ejecutarán manualmente Camila o Jonatan._

_Última revisión documental: 2026-09-16._

## Objetivo

Comparar las tres finalistas con el mismo caso de uso y medir la complejidad operativa real para una persona no técnica.

No buscamos la plataforma con más funciones, sino la que permita operar correctamente con la menor complejidad y costo total razonables.

## Reglas

- Las cuentas de prueba se crean manualmente por Camila o Jonatan.
- Usar datos ficticios siempre que sea posible.
- No guardar contraseñas, tokens, credenciales, CUIT ni datos bancarios en GitHub.
- No contratar planes pagos ni generar cargos sin aprobación explícita de `@JonatanGarbuyo`.
- Si una integración exige una cuenta real del comercio, marcarla `PENDIENTE CON TITULAR`.

## Gates obligatorios

Una plataforma no puede elegirse si falla sin alternativa simple y segura:

1. acceso separado para comercio + Camila sin compartir contraseña;
2. talles, colores y stock por variante;
3. checkout autoservicio con pago local y envío nacional;
4. operación diaria entendible para Camila sin desarrollo.

## Cómo medir fragmentación

### Pagos

Registrar si para cobrar, conciliar, devolver o reintegrar dinero hay que salir del panel principal de la tienda.

Eso **no es automáticamente malo**. La pregunta es si Camila y el comercio aceptan esa separación del flujo y si la trazabilidad sigue siendo clara.

El criterio es independiente del proveedor de pago.

### Envíos

Registrar si para generar etiquetas, despachar, consultar tracking, cancelar o resolver incidencias hay que usar otro panel.

La fragmentación logística pesa más negativamente porque esas tareas forman parte del trabajo operativo cotidiano.

## Mini catálogo común

Usar los mismos productos en las tres plataformas:

### Producto A — Remera básica algodón

- precio: ARS 20.000;
- colores: negro y blanco;
- talles: S, M, L;
- stock diferente por combinación;
- SKU por variante;
- peso: 0,30 kg.

### Producto B — Jean recto azul

- precio: ARS 45.000;
- talles 36, 38, 40, 42;
- stock por talle;
- peso: 0,70 kg.

### Producto C — Cinturón negro

- precio: ARS 15.000;
- sin variantes;
- stock: 3;
- peso: 0,20 kg.

## Contenido común

Crear:

- categorías `Remeras` y `Jeans`;
- página `Envíos`;
- página `Cambios y devoluciones`;
- página `Contacto`;
- WhatsApp si puede configurarse sin usar datos sensibles.

Para publicación/SEO usar [`/wiki/publicacion-y-seo.md`](../../wiki/publicacion-y-seo.md).

## Pruebas

### 1. Alta inicial

Registrar:

- tiempo de alta;
- si exige tarjeta;
- datos requeridos;
- subdominio;
- claridad del asistente inicial.

### 2. Producto y variantes

- crear la remera;
- cargar color + talle;
- stock distinto por combinación;
- dejar una variante sin stock;
- cargar SKU, peso y dimensiones;
- cambiar stock y precio;
- observar comportamiento público.

### 3. Stock agotado

Simular una venta física y actualizar una variante. Verificar rapidez, claridad y riesgo de sobreventa.

### 4. Publicación y SEO

Aplicar la guía de `/wiki/publicacion-y-seo.md` y comprobar qué campos existen y cuáles automatiza la plataforma.

### 5. Accesos

Intentar crear:

- `Propietario`;
- `Operador` (Camila).

Verificar permisos, acceso a configuración sensible y posibilidad de revocar al operador sin cambiar la contraseña del propietario.

### 6. Pago

Validar hasta donde sea seguro:

- checkout;
- cambio de estado de pago;
- conciliación;
- devolución/reintegro;
- trazabilidad entre tienda y proveedor de pago;
- cantidad de paneles utilizados.

Registrar si la fragmentación de pago resulta aceptable o incómoda para Camila/comercio.

### 7. Envío

Verificar:

- cotización;
- domicilio/sucursal;
- etiqueta;
- impresión;
- tracking;
- cancelación;
- seguro;
- cantidad de paneles utilizados.

Penalizar especialmente la necesidad habitual de operar otro panel para estas tareas.

### 8. Pedido, cancelación y reintegro

Comprobar pedido, pago, stock, cancelación, restauración de stock y evidencia de reintegro.

### 9. Métricas y atribución

Usar un enlace con UTM y verificar si puede distinguirse fuente/campaña y revenue cuando corresponda.

### 10. Portabilidad

Verificar exportación de productos, ventas, clientes y reportes.

### 11. Móvil

Desde teléfono:

`producto → variante → carrito → envío → pago`

Registrar fricciones.

### 12. Operación diaria

Simular:

1. revisar tres pedidos;
2. actualizar dos stocks;
3. cambiar un precio;
4. identificar pedidos pagos;
5. preparar un envío;
6. buscar un cliente;
7. cancelar una orden;
8. consultar una métrica.

Registrar tiempo, paneles abiertos y tutoriales necesarios.

## Hoja de resultados

Por plataforma completar:

| Prueba | Estado | Tiempo | Paneles | Observación |
| --- | --- | ---: | ---: | --- |
| Alta inicial | PENDIENTE | — | — | |
| Producto/variantes | PENDIENTE | — | — | |
| Stock agotado | PENDIENTE | — | — | |
| Publicación/SEO | PENDIENTE | — | — | |
| Accesos | PENDIENTE | — | — | |
| Pago | PENDIENTE | — | — | |
| Envío | PENDIENTE | — | — | |
| Cancelación/reintegro | PENDIENTE | — | — | |
| Métricas | PENDIENTE | — | — | |
| Portabilidad | PENDIENTE | — | — | |
| Móvil | PENDIENTE | — | — | |
| Operación diaria | PENDIENTE | — | — | |

Usar `PASS`, `WARN`, `FAIL` o `PENDIENTE`.

Al terminar, actualizar `docs/research/shortlist-plataformas.md` y dejar #19 listo para cerrar. La selección final sigue en #9.