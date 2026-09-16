# Protocolo de prueba — Tiendanube vs DonWeb vs Empretienda

[← Índice de investigación](README.md) · [Índice general](../INDEX.md) · [Shortlist](shortlist-plataformas.md)

_Estado: protocolo listo. La prueba práctica en paneles sigue pendiente._

_Última revisión documental: 2026-09-16._

## Objetivo

Comparar las tres finalistas con el **mismo caso de uso**, midiendo complejidad operativa real para una persona no técnica. La prueba no busca encontrar la plataforma con más funciones, sino la que permita operar la tienda de ropa con la menor complejidad y costo total razonables.

Plataformas:

1. Tiendanube
2. DonWeb SitioSimple
3. Empretienda

La decisión final no se toma en este documento. Vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.

## Reglas de seguridad y costo

- Usar exclusivamente datos ficticios en las tiendas de prueba.
- No guardar contraseñas, tokens, API keys, CUIT, datos bancarios ni credenciales en GitHub.
- No usar tarjetas personales para una prueba cuando no sea indispensable.
- No contratar planes pagos ni generar cargos sin aprobación explícita de `@JonatanGarbuyo`.
- Si una integración exige una cuenta real del comercio, marcarla como `PENDIENTE CON TITULAR` en vez de inventar datos.
- No compartir una contraseña entre el dueño del comercio y Camila. Si la plataforma no ofrece acceso delegado legítimo, registrarlo como riesgo/bloqueo.

## Resultado por prueba

Usar una de estas marcas:

- `PASS`: cubre el caso sin workaround relevante.
- `WARN`: cubre el caso, pero agrega pasos, restricciones o trabajo manual aceptable solo a bajo volumen.
- `FAIL`: bloquea un requisito del MVP o exige una práctica insegura/no aceptable.
- `PENDIENTE`: no puede verificarse sin cuenta/credencial real del comercio.

Además registrar:

- tiempo aproximado para completar la tarea;
- cantidad de pantallas/paneles externos necesarios;
- cualquier paso que un operador no técnico probablemente necesite documentar en el playbook.

## Gates obligatorios

Una plataforma no puede ser elegida para el MVP si falla alguno de estos puntos sin alternativa simple y segura.

### Gate A — acceso seguro

Debe existir una forma aceptable de que el comercio sea titular y Camila administre sin compartir contraseñas personales.

- Ideal: usuario propio con permisos limitados.
- Aceptable para piloto: usuario propio con acceso total, si los dueños lo aprueban explícitamente.
- No aceptable: una única contraseña personal compartida entre dueño y administradora.

### Gate B — catálogo de indumentaria

Debe poder manejar, como mínimo:

- talle;
- color;
- stock por combinación;
- SKU o identificador;
- peso/dimensiones suficientes para cotizar envío;
- agotado/oculto sin romper el producto completo.

### Gate C — venta autoservicio

Un comprador debe poder completar:

`producto → variante → carrito → datos → pago → envío → confirmación`

sin conversar por WhatsApp ni requerir intervención manual antes de pagar.

### Gate D — operación diaria

Camila debe poder entender y ejecutar sin desarrollo:

- ver pedidos pendientes;
- distinguir pago pendiente/pagado;
- preparar envío;
- actualizar stock/precio;
- cancelar pedido;
- iniciar o registrar reintegro;
- consultar cliente;
- resolver incidencias comunes.

## Mini catálogo común

Usar exactamente estos productos ficticios o equivalentes en las tres plataformas.

### Producto A — Remera Básica Algodón

- Precio: ARS 20.000
- Categoría: Remeras
- SKU base: `TEST-REMERA`
- Variantes:
  - Color: Negro, Blanco
  - Talle: S, M, L
- Stock:
  - Negro/S: 2
  - Negro/M: 1
  - Negro/L: 0
  - Blanco/S: 1
  - Blanco/M: 2
  - Blanco/L: 1
- Peso: 0,30 kg
- Dimensiones de paquete de prueba: 30 × 25 × 5 cm

Objetivo: probar combinación de dos atributos y stock independiente por variante.

### Producto B — Jean Recto Azul

- Precio: ARS 45.000
- Categoría: Jeans
- Talles: 36, 38, 40, 42
- Stock total repartido entre talles
- Peso: 0,70 kg

Objetivo: probar una sola propiedad de variante y edición rápida de stock/precio.

### Producto C — Gift card / accesorio simple

Usar un producto sin variantes, por ejemplo:

- Nombre: Cinturón Negro
- Precio: ARS 15.000
- Stock: 3
- Peso: 0,20 kg

Objetivo: medir el camino mínimo de alta de un producto sencillo.

## Contenido común

Crear:

- categoría `Remeras`;
- categoría `Jeans`;
- página `Envíos`;
- página `Cambios y devoluciones`;
- página `Contacto`;
- botón/enlace de WhatsApp con número ficticio o sin publicar si exige un número real.

Para SEO usar el procedimiento de [`../playbook/04-seo-y-publicacion.md`](../playbook/04-seo-y-publicacion.md).

## Prueba 1 — alta inicial

Registrar:

- cuánto tarda crear la tienda;
- si exige tarjeta para iniciar;
- qué datos fiscales/comerciales exige antes de poder explorar el panel;
- si el trial/free tier permite publicar una tienda funcional;
- subdominio asignado;
- claridad del asistente inicial.

### Pre-validación documental

- **Tiendanube:** plan Inicial permanente de costo fijo $0; se puede operar con subdominio `*.mitiendanube.com`.
- **DonWeb:** prueba de 15 días, publicada como sin tarjeta; luego plan Tienda pago.
- **Empretienda:** página comercial vigente publica 15 días gratis sin configurar método de pago. Sus términos públicos todavía mencionan 30 días; tomar la página comercial vigente como condición operativa a confirmar al crear la cuenta.

## Prueba 2 — producto y variantes

Para la Remera:

1. crear producto;
2. agregar color y talle como propiedades separadas;
3. cargar stock diferente en cada combinación;
4. dejar Negro/L sin stock;
5. asignar SKU;
6. cargar peso/dimensiones;
7. comprobar desde storefront qué ocurre con una variante agotada;
8. cambiar stock de Negro/M de 1 a 3;
9. registrar tiempo y cantidad de clics/pantallas aproximada.

### Pre-validación documental

- **Tiendanube:** documenta variantes por propiedades, generación automática de combinaciones y stock/precio/peso/SKU por variante. El plan Inicial no permite carga masiva.
- **Empretienda:** documenta atributos/variantes, stock/SKU y carga/importación masiva; la página comercial vigente también publica gestión de productos y stock.
- **DonWeb:** publica catálogo, stock y edición/importación vía planilla; verificar en panel actual la profundidad exacta de variantes y la edición masiva en la versión nueva.

## Prueba 3 — stock agotado y venta física paralela

Simular que una unidad se vendió en el local físico:

1. modificar el stock de una variante;
2. comprobar cuánto tarda en reflejarse públicamente;
3. verificar si la plataforma permite ocultar una combinación agotada sin borrar las restantes;
4. observar si existe historial o señal suficiente para evitar errores.

Registrar especialmente cualquier riesgo de sobreventa si el stock también vive en otro sistema del local.

## Prueba 4 — SEO/publicación

Aplicar al Producto A:

- título comercial claro;
- descripción original;
- título SEO;
- meta description;
- URL amigable;
- texto alternativo en imagen cuando esté disponible;
- categoría;
- indexabilidad/sitemap;
- feed de Google Shopping, sin necesidad de publicarlo si exige cuenta real.

Resultado esperado: verificar qué parte del procedimiento se puede controlar y qué parte automatiza la plataforma.

## Prueba 5 — acceso Camila + dueño

Crear, si la plataforma lo permite, dos identidades separadas:

- `Propietario` — titular de cuenta/facturación/cobros.
- `Operador` — Camila, administración diaria.

Verificar:

- creación de usuario adicional;
- permisos configurables;
- acceso a productos;
- ventas;
- pagos;
- envíos;
- configuración sensible;
- facturación/plan;
- posibilidad de desactivar el usuario sin cambiar la contraseña del propietario.

### Pre-validación documental

- **DonWeb:** PASS documental. SitioSimple documenta usuarios con permisos por sección, activación/desactivación y vista previa de permisos.
- **Tiendanube Inicial:** WARN documental. Admite varios usuarios, pero en Inicial todos tienen acceso total; permisos granulares requieren un plan que los incluya.
- **Empretienda:** PENDIENTE / riesgo. No se encontró documentación pública actual de colaboradores. Sus términos indican que cuenta y contraseña son personales, secretas e intransferibles; no usar password compartido como workaround.

## Prueba 6 — pago

Configurar hasta donde sea seguro sin credenciales reales.

### Tiendanube

Validar Pago Nube:

- métodos visibles;
- flujo dentro del checkout;
- pantalla de transacciones;
- conciliación/reporting;
- devolución/reintegro desde administración.

Documentalmente, Pago Nube centraliza pagos, devoluciones, contracargos y reportes en Tiendanube.

### DonWeb

Validar Mercado Pago como caso principal:

- configuración requerida;
- redirección a Mercado Pago;
- retorno a la tienda;
- estado de la orden después del pago;
- qué parte del reintegro debe hacerse en Mercado Pago y qué parte en SitioSimple.

Documentalmente, SitioSimple requiere credenciales de Mercado Pago y redirige al comprador al proveedor para pagar.

### Empretienda

Validar Mercado Pago y transferencia:

- configuración;
- actualización automática/manual del estado;
- devolución/reintegro;
- conciliación;
- cuánto del flujo ocurre fuera del panel.

Si requiere una cuenta comercial real, marcar la integración como `PENDIENTE CON TITULAR` y continuar con un método manual de prueba.

## Prueba 7 — envío

Usar el origen ficticio definido para la prueba hasta conocer el origen real del comercio.

Verificar:

- cotización en checkout;
- domicilio;
- sucursal/punto de retiro si existe;
- creación/pago de etiqueta;
- impresión;
- tracking;
- cancelación;
- seguro;
- cantidad de paneles necesarios.

### Pre-validación documental

- **Tiendanube Inicial:** Andreani/Envío Nube centraliza buena parte de la operación en el administrador.
- **DonWeb:** permite Andreani, OCA, Envia.com, retiro, método propio y a convenir. Con Envia.com la tienda calcula/ofrece tarifas, pero la gestión efectiva del envío se realiza en la cuenta de Envia.com. Andreani/OCA pueden requerir cuenta propia.
- **Empretienda:** publica OCA, Correo Argentino, Andreani, E-Pick y métodos personalizados; validar en panel qué operaciones se centralizan y cuáles exigen portales externos.

## Prueba 8 — pedido, cancelación y reintegro

Crear una orden de prueba cuando pueda hacerse sin cargo real o usar el flujo más cercano disponible.

Verificar:

1. notificación de venta;
2. lista de pedidos;
3. estado de pago;
4. estado de preparación/envío;
5. cancelación;
6. restauración de stock;
7. reintegro;
8. evidencia de que el reintegro ocurrió;
9. qué sistema conserva la trazabilidad.

En Tiendanube, documentar por separado `cancelar venta` y `devolver dinero`: no siempre son la misma acción.

## Prueba 9 — métricas y atribución

Agregar un enlace de prueba con:

`utm_source=instagram&utm_medium=organic_social&utm_campaign=piloto&utm_content=producto_a`

Verificar:

- si la visita aparece en analítica disponible;
- integración con Google Analytics;
- Pixel/Meta;
- evento de compra/revenue cuando pueda probarse;
- posibilidad de distinguir fuente/campaña;
- facilidad para construir el reporte semanal definido en `measurement.md`.

No puntuar positivamente solo por tener un dashboard propio: necesitamos poder responder de dónde llegó una venta.

## Prueba 10 — portabilidad

Verificar sin datos reales:

- exportar productos;
- exportar ventas;
- exportar clientes;
- recuperar imágenes/contenido;
- descargar reportes de pagos;
- facilidad para migrar a otra plataforma.

Una plataforma con costo bajo pero fuerte lock-in debe quedar marcada `WARN`.

## Prueba 11 — experiencia móvil

Realizar desde un teléfono o emulación móvil:

- abrir home;
- encontrar Producto A;
- elegir color/talle;
- agregar al carrito;
- avanzar checkout;
- calcular envío;
- llegar al método de pago;
- volver al carrito y editar variante/cantidad.

Registrar fricción visible, pasos redundantes, elementos difíciles de tocar o cualquier necesidad de asistencia por WhatsApp para completar la compra.

## Prueba 12 — carga operativa diaria

Simular una mañana de operación:

1. revisar tres pedidos;
2. cambiar stock de dos variantes;
3. cambiar un precio;
4. responder qué pedidos están pagos;
5. preparar un envío;
6. buscar un cliente;
7. cancelar una orden;
8. consultar una métrica de ventas.

Medir:

- tiempo total;
- paneles abiertos;
- credenciales/cuentas externas utilizadas;
- puntos donde fue necesario consultar un tutorial;
- puntos que deben convertirse en procedimiento del playbook.

## Hoja de resultados

Completar una tabla por plataforma:

| Prueba | Estado | Tiempo | Paneles | Observación |
| --- | --- | ---: | ---: | --- |
| Alta inicial | PENDIENTE | — | — | |
| Producto/variantes | PENDIENTE | — | — | |
| Stock agotado | PENDIENTE | — | — | |
| SEO/publicación | PENDIENTE | — | — | |
| Accesos | PENDIENTE | — | — | |
| Pago | PENDIENTE | — | — | |
| Envío | PENDIENTE | — | — | |
| Cancelación/reintegro | PENDIENTE | — | — | |
| Métricas/atribución | PENDIENTE | — | — | |
| Portabilidad | PENDIENTE | — | — | |
| Móvil | PENDIENTE | — | — | |
| Operación diaria | PENDIENTE | — | — | |

## Criterio de salida

Al terminar, actualizar [`shortlist-plataformas.md`](shortlist-plataformas.md) con hechos observados y dejar #19 listo para cerrar.

La plataforma candidata a #9 debe:

1. pasar los cuatro gates;
2. no requerir prácticas inseguras;
3. ser operable por Camila sin desarrollo;
4. tener costo total razonable para el volumen inicial;
5. tener una ruta clara para crecer sin rehacer toda la operación demasiado pronto.
