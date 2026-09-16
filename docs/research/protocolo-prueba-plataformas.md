# Protocolo de prueba — Tiendanube vs DonWeb

_Estado: protocolo listo. La prueba práctica en paneles la ejecutarán manualmente Camila o Jonatan._

_Última revisión documental: 2026-09-16._

## Objetivo

Comparar **Tiendanube** y **DonWeb SitioSimple** con el mismo caso de uso, midiendo complejidad operativa real para una persona no técnica.

Empretienda quedó fuera de la evaluación activa. Ver `shortlist-plataformas.md`.

## Reglas

- Usar datos ficticios.
- No guardar contraseñas, tokens, CUIT, datos bancarios ni credenciales en GitHub.
- No contratar planes pagos ni generar cargos sin aprobación explícita de `@JonatanGarbuyo`.
- Si una integración requiere una cuenta real del comercio, marcar `PENDIENTE CON TITULAR`.

## Gates obligatorios

Una finalista no puede elegirse si falla sin alternativa simple y segura en alguno de estos puntos:

1. acceso separado comercio + Camila sin compartir contraseña;
2. variantes y stock de indumentaria;
3. checkout autoservicio con pago local;
4. envío nacional;
5. operación diaria entendible para Camila sin desarrollo.

## Fragmentación

### Pagos

Registrar si cobros, conciliación, devoluciones o reintegros requieren un panel distinto al panel principal de la tienda.

La fragmentación de pagos **puede ser aceptable** si Camila y el comercio consideran el flujo claro y manejable. El criterio no depende del proveedor.

### Envíos

Registrar si etiquetas, despacho, tracking o incidencias requieren otro panel.

La fragmentación habitual de envíos se considera una **desventaja fuerte** porque afecta la operación cotidiana.

## Mini catálogo común

Cargar en ambas plataformas los mismos productos ficticios:

- Remera básica de algodón con 2 colores × 3 talles y stock distinto por combinación.
- Jean recto con talles 36, 38, 40 y 42.
- Accesorio simple sin variantes.

Agregar también:

- categorías;
- página de envíos;
- página de cambios/devoluciones;
- página de contacto;
- WhatsApp cuando pueda configurarse sin exponer datos reales;
- SEO siguiendo `../../wiki/publicacion-y-seo.md`.

## Pruebas

En cada plataforma ejecutar y registrar:

1. **Alta inicial** — claridad del onboarding, datos requeridos y límites del plan/trial.
2. **Productos y variantes** — alta, talle/color, stock por combinación, SKU, peso/dimensiones.
3. **Stock** — cambio de stock y comportamiento de variantes agotadas.
4. **SEO/publicación** — título, descripción, URL, categorías, sitemap y controles disponibles.
5. **Accesos** — propietario + operador; permisos y revocación del acceso.
6. **Pagos** — configuración, estado de orden, conciliación, cancelación y reintegro.
7. **Envíos** — cotización, etiqueta, despacho, tracking, cancelación e incidencias.
8. **Pedido completo** — compra hasta donde pueda probarse sin cargos innecesarios.
9. **Métricas** — Analytics/Pixel/UTMs y trazabilidad de fuente de venta.
10. **Portabilidad** — exportación de productos, ventas y clientes cuando exista.
11. **Móvil** — producto → variante → carrito → envío → pago.
12. **Operación diaria** — revisar pedidos, cambiar stock/precio, preparar envío, cancelar una orden y consultar ventas.

## Hoja de resultados

Usar `PASS`, `WARN`, `FAIL` o `PENDIENTE`.

| Prueba | Tiendanube | DonWeb | Observación |
| --- | --- | --- | --- |
| Alta inicial | PENDIENTE | PENDIENTE | |
| Productos/variantes | PENDIENTE | PENDIENTE | |
| Stock | PENDIENTE | PENDIENTE | |
| SEO/publicación | PENDIENTE | PENDIENTE | |
| Accesos | PENDIENTE | PENDIENTE | |
| Pagos | PENDIENTE | PENDIENTE | |
| Envíos | PENDIENTE | PENDIENTE | |
| Cancelación/reintegro | PENDIENTE | PENDIENTE | |
| Métricas | PENDIENTE | PENDIENTE | |
| Portabilidad | PENDIENTE | PENDIENTE | |
| Móvil | PENDIENTE | PENDIENTE | |
| Operación diaria | PENDIENTE | PENDIENTE | |

## Salida

Al completar la prueba:

1. actualizar `shortlist-plataformas.md` con hechos observados;
2. cerrar #19 si la evidencia es suficiente;
3. llevar la comparación final a #9 para aprobación de `@JonatanGarbuyo`.
