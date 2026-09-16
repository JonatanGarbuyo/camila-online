# Wayfinder map — Tienda online nacional de bajo costo para Camila

## Destination

Llegar a una especificación de MVP y un plan de lanzamiento claros para que Camila pueda crear y administrar una tienda online en Argentina con catálogo, checkout/pago online, logística, WhatsApp, SEO/publicación y medición.

Este mapa es interno al proyecto: **no forma parte de la guía para operadores no técnicos**.

## Separación de documentación

- `docs/INDEX.md`: portada simple para Camila/operadores. Solo procedimientos y conocimiento práctico.
- `docs/playbook/`: manual operativo reusable.
- `docs/research/`: investigación y evidencia interna.
- `docs/wayfinder/` + Issues: decisiones, estado, bloqueos y discovery.

No agregar Wayfinder, Issues ni research interno al índice operativo.

## Decisiones / research vigente

- MVP no-code.
- Venta autoservicio principal; WhatsApp como asistencia humana.
- Catálogo inicialmente administrable de forma manual.
- Dominio propio nice-to-have.
- Shortlist activa: **Tiendanube, DonWeb SitioSimple y Empretienda**.
- La plataforma final todavía no está decidida.
- Tiendanube Inicial: costo fijo $0 y flujo local muy integrado; restricciones en dominio, carga masiva, proveedores y permisos.
- DonWeb: costo bajo, permisos diferenciados y potencial futuro multi-comercio; principal riesgo = fragmentación operativa.
- Empretienda: opción local simple; pendiente verificar acceso delegado/multiusuario.
- Fragmentación de **pagos** puede ser aceptable si el comercio ya usa Mercado Pago y quiere conservarlo.
- Fragmentación de **envíos** pesa negativamente si obliga a operar habitualmente otro panel para etiquetas, despacho o tracking.
- Las cuentas de prueba de plataformas se crean y operan manualmente por Camila o Jonatan.

## Frontier

### #6 — operación diaria, stock, despacho y fragmentación

Handoff a Camila. Relevar además:

- si el comercio ya usa Mercado Pago;
- si desea conservar esa cuenta;
- si Camila acepta operar pagos en un panel externo;
- cuánta fragmentación tolera;
- si para envíos acepta o no un panel externo cotidiano.

### #7 — catálogo, variantes y política de stock

Handoff a Camila.

### #13 — titularidad, facturación y accesos

Handoff a Camila.

### #19 — prueba manual Tiendanube / DonWeb / Empretienda

Camila o Jonatan ejecutan manualmente `docs/research/protocolo-prueba-plataformas.md` usando datos ficticios.

## Blocked

- #8 — cambios, devoluciones y logística inversa — depende de #6 y #7.
- #9 — elegir plataforma del MVP — depende de #6, #7, #8, #13 y #19. Requiere aprobación explícita de `@JonatanGarbuyo`.
- #10 — modelo comercial del servicio — depende de #6 y #9.
- #15 — completar playbook operativo — depende de operación y plataforma elegida.

## Out of scope

- E-commerce custom ahora.
- SaaS multi-tenant ahora.
- Automatizaciones complejas antes de validar volumen y dolor operativo.