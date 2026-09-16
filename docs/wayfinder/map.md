# Wayfinder map — Tienda online nacional de bajo costo para Camila

## Destination

Llegar a una especificación de MVP y un plan de lanzamiento suficientemente claros para que Camila pueda crear y administrar una tienda online en Argentina, vendiendo a todo el país con catálogo, checkout/pago online, logística, WhatsApp, SEO/publicación y medición.

El resultado de este mapa es **decisión y especificación, no implementación productiva**.

## Notes

- Primer caso real: negocio existente de ropa.
- MVP no-code.
- Camila será la responsable operativa.
- Venta principal autoservicio; WhatsApp como asistencia humana.
- Catálogo/stock puede comenzar manual.
- Dominio propio es nice-to-have.
- `/wiki/` es la guía operativa para personas no técnicas.
- `docs/` queda para research, Wayfinder y documentación interna.
- #6, #7 y #13 son handoff a Camila.

## Decisions / research so far

- Shortlist activa: **Tiendanube, DonWeb SitioSimple y Empretienda**.
- Tiendanube Inicial: $0 y flujo local integrado; restricciones de dominio, carga masiva, proveedores y permisos.
- DonWeb: costo bajo, permisos diferenciados y potencial multi-comercio; hay que validar fragmentación operativa.
- Empretienda: opción local simple; falta validar acceso delegado/multiusuario.
- **Fragmentación de pagos:** evaluar si Camila y el comercio aceptan que cobros, conciliación, devoluciones o reintegros se operen parcialmente en un panel separado del panel principal de la tienda. El criterio es independiente del proveedor de pago.
- **Fragmentación de envíos:** pesa negativamente si la operación normal obliga a usar habitualmente otro panel para generar etiquetas, despachar o seguir pedidos.
- Las pruebas de cuentas/plataformas las ejecutarán manualmente Camila o Jonatan.

## Frontier

- #6 — operación diaria, stock, despacho y tolerancia a fragmentación — responder con Camila.
- #7 — catálogo, variantes y política de stock — responder con Camila.
- #13 — titularidad, facturación y accesos — responder con Camila.
- #19 — prueba manual comparable de Tiendanube, DonWeb y Empretienda.

## Blocked

- #8 — cambios, devoluciones y logística inversa — blocked by #6 y #7.
- #9 — elegir plataforma del MVP — blocked by #6, #7, #8, #13 y #19; requiere aprobación explícita de `@JonatanGarbuyo`.
- #10 — modelo comercial del servicio — blocked by #6 y #9.
- #15 — completar wiki operativa — depende de operación/plataforma.

## Closed research / tasks

- #2, #3, #4, #5, #11, #12, #14, #16, #17 cerrados.
- #18 GitHub Wiki diferida; se usa `/wiki/` dentro del repo.

## Out of scope

- E-commerce custom ahora.
- SaaS multi-tenant ahora.
- Automatizaciones complejas antes de validar volumen y dolor operativo.
