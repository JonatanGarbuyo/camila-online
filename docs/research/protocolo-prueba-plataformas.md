# Protocolo de prueba — Tiendanube vs DonWeb vs Empretienda

_Estado: listo para ejecutar manualmente._

Las cuentas de prueba se crean y operan **manualmente por Camila o Jonatan**. No automatizar altas ni guardar credenciales reales en GitHub.

## Objetivo

Comparar las tres finalistas con el mismo caso de uso y medir complejidad operativa real.

No buscamos la plataforma con más funciones, sino la que permita operar la tienda con la menor complejidad y costo total razonables.

## Reglas

- Usar datos ficticios.
- No guardar contraseñas, tokens, CUIT, datos bancarios ni credenciales.
- No contratar planes pagos ni generar cargos sin aprobación explícita.
- Si una integración exige una cuenta real del comercio, marcar `PENDIENTE CON TITULAR`.
- No compartir una contraseña entre dueño y Camila.

## Estados

- `PASS`: cubre el caso sin workaround relevante.
- `WARN`: funciona, pero agrega pasos o trabajo manual.
- `FAIL`: bloquea un requisito o exige una práctica insegura/no aceptable.
- `PENDIENTE`: requiere cuenta/credencial real del comercio.

Registrar además tiempo aproximado, cantidad de paneles utilizados y observaciones.

## Gates obligatorios

### 1. Acceso seguro

El comercio debe poder ser titular y Camila operar sin compartir contraseña.

### 2. Catálogo de ropa

Debe manejar talle, color, stock por combinación, SKU, precio y datos de envío.

### 3. Venta autoservicio

El comprador debe completar:

`producto → variante → carrito → datos → pago → envío → confirmación`

sin intervención humana obligatoria.

### 4. Operación diaria

Camila debe poder ver pedidos, distinguir pagos, preparar envíos, actualizar stock/precio, cancelar pedidos, registrar reintegros y resolver incidencias sin desarrollo.

## Catálogo ficticio común

### Producto A — Remera Básica Algodón

- ARS 20.000
- colores: Negro, Blanco
- talles: S, M, L
- stock diferente por combinación
- una combinación agotada
- peso: 0,30 kg
- paquete: 30 × 25 × 5 cm

### Producto B — Jean Recto Azul

- ARS 45.000
- talles 36, 38, 40, 42
- stock por talle
- peso: 0,70 kg

### Producto C — Cinturón Negro

- ARS 15.000
- sin variantes
- stock: 3
- peso: 0,20 kg

Crear además categorías, página de envíos, cambios/devoluciones y contacto.

## Pruebas

### Alta

Registrar si pide tarjeta, qué datos exige, subdominio disponible y claridad del onboarding.

### Producto y variantes

Crear la remera con color+talle, stock por combinación, SKU, peso y una variante agotada. Luego modificar stock y precio.

### SEO/publicación

Aplicar el procedimiento de `../playbook/04-seo-y-publicacion.md`: título, descripción, categoría, title/meta, URL, imágenes y sitemap/indexación cuando corresponda.

### Accesos

Crear dos identidades si es posible:

- Propietario
- Operador (Camila)

Verificar qué puede hacer cada una y si el operador puede desactivarse sin cambiar la contraseña del propietario.

### Pago

Validar el flujo hasta donde sea seguro sin credenciales reales.

**Separar fragmentación de pago de fragmentación logística.**

Un panel externo de Mercado Pago puede ser aceptable si el comercio ya usa esa cuenta y Camila está cómoda operándola para conciliaciones/reintegros.

Registrar:

- dónde se configura;
- dónde se consulta la transacción;
- dónde se hace un reintegro;
- si el estado vuelve correctamente a la tienda;
- si hay conciliación manual.

### Envío

Este punto pesa especialmente en la decisión.

Verificar:

- cotización en checkout;
- generación/pago de etiqueta;
- impresión;
- tracking;
- cancelación;
- seguro;
- cantidad de paneles utilizados.

**WARN fuerte** si para cada pedido hay que entrar habitualmente a otro panel para generar etiquetas, despachar o seguir el envío.

### Pedido, cancelación y reintegro

Verificar notificación, estado de pago, estado de envío, cancelación, restauración de stock y trazabilidad del reintegro.

### Métricas

Usar un enlace con UTM y comprobar si puede identificarse fuente/campaña y revenue cuando el trial lo permita.

### Portabilidad

Verificar exportación de productos, ventas, clientes, imágenes/reportes cuando exista.

### Móvil

Probar búsqueda, variante, carrito, checkout, envío y pago desde teléfono.

### Operación diaria simulada

Simular:

1. revisar tres pedidos;
2. cambiar stock de dos variantes;
3. cambiar un precio;
4. identificar pedidos pagos;
5. preparar un envío;
6. buscar un cliente;
7. cancelar una orden;
8. consultar una métrica.

Registrar tiempo total y paneles abiertos.

## Hoja de resultados

| Prueba | Estado | Tiempo | Paneles | Observación |
| --- | --- | ---: | ---: | --- |
| Alta | PENDIENTE | — | — | |
| Producto/variantes | PENDIENTE | — | — | |
| SEO/publicación | PENDIENTE | — | — | |
| Accesos | PENDIENTE | — | — | |
| Pago | PENDIENTE | — | — | |
| Envío | PENDIENTE | — | — | |
| Cancelación/reintegro | PENDIENTE | — | — | |
| Métricas | PENDIENTE | — | — | |
| Portabilidad | PENDIENTE | — | — | |
| Móvil | PENDIENTE | — | — | |
| Operación diaria | PENDIENTE | — | — | |

## Criterio de salida

Actualizar `shortlist-plataformas.md` con hechos observados. La prueba produce evidencia; la decisión final de plataforma se toma aparte y requiere aprobación de `@JonatanGarbuyo`.