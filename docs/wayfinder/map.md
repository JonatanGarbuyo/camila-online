# Wayfinder map — Tienda online nacional de bajo costo para Camila

[← Índice de documentación](../INDEX.md)

## Destination

Llegar a una especificación de MVP y un plan de lanzamiento suficientemente claros para que Camila pueda crear y administrar una tienda online en Argentina, vendiendo a todo el país con el menor costo fijo razonable, con catálogo, checkout/pago online, logística con cobertura/seguro, atención por WhatsApp, SEO/publicación y medición de adquisición/conversión.

El resultado de este mapa es **decisión y especificación, no implementación productiva**.

## Notes

- Primer caso real: negocio existente de **ropa**.
- El MVP será **no-code**; no desarrollar software propio mientras una solución administrada cubra razonablemente el problema.
- Camila será la **responsable operativa** y administrará la tienda online.
- Jonatan aporta tecnología/desarrollo; los procesos del negocio que no conoce deben relevarse con Camila, no inferirse.
- Venta principal **autoservicio end-to-end**; WhatsApp como asistencia humana.
- El catálogo/stock puede comenzar con administración manual.
- Prioridad: costo fijo nulo o bajo, evaluando costo total real y carga operativa.
- Subdominio gratuito aceptable durante validación; **dominio propio es nice-to-have**.
- El repo es base de conocimiento canónica. La navegación principal de la “wiki en Markdown” vive en `docs/INDEX.md`.
- `docs/playbook/` es la fuente del manual operativo; por ahora no se mantiene una copia en GitHub Wiki.
- Toda la documentación durable se mantiene en archivos Markdown en español dentro del repo.
- Posible servicio futuro para otros comercios, sin construir ahora un SaaS genérico.
- Investigación con fuentes primarias y condiciones vigentes para Argentina.
- #6, #7 y #13 son handoff a Camila.

## Decisions / research so far

- **MVP no-code** y **venta autoservicio principal**.
- **Atención humana por WhatsApp**; bots/IA quedan fuera del MVP.
- **Dominio propio nice-to-have**; no bloquea lanzamiento.
- **Shortlist activa de plataforma:** Tiendanube, DonWeb SitioSimple y Empretienda. La plataforma final todavía no está decidida.
- **Fuera de evaluación activa:** Shopify, Wix, Odoo y otras alternativas; solo reabrirlas si las tres finalistas quedan bloqueadas por una restricción concreta.
- **Tiendanube Inicial:** $0 de costo fijo y flujo local muy integrado; restricciones relevantes en carga/exportación masiva, dominio, medios de pago/envío y permisos granulares.
- **Tiendanube Esencial no incluye el dominio:** habilita a conectar uno propio, que se compra/renueva aparte.
- **DonWeb SitioSimple:** research documental confirma pagos/envíos locales, carga masiva, dominio, SEO y usuarios con permisos diferenciados. Su modalidad Revendedores/Partners puede facilitar un servicio futuro para varios comercios. Research: `docs/research/donweb-sitiosimple.md`.
- **Riesgo DonWeb:** comprobar en práctica que la libertad de integrar Mercado Pago/Andreani/OCA/Envia.com no fragmente el día a día entre demasiados paneles.
- **Empretienda:** un único plan simple con muchas funciones locales; falta verificar especialmente acceso multiusuario/permisos para que Camila no tenga que compartir credenciales con el comercio.
- **Pagos:** Pago Nube cubre tarjeta/débito/MODO + transferencia en Tiendanube Inicial.
- **Logística:** Andreani/Envío Nube cubre el MVP nacional de ropa; cambios/devoluciones requieren flujo separado.
- **Medición:** UTMs + GA4 + Meta Pixel/CAPI en Tiendanube; las equivalencias deben validarse en las otras finalistas.
- **Consumo/devoluciones:** ventas a distancia tienen derecho de arrepentimiento; verificar implementación vigente del botón antes de lanzar.
- **Facturación/titularidad:** propuesta a validar: tienda/cobros/facturación a nombre del comercio; Camila administra el canal y cobra su servicio aparte.
- **WhatsApp/redes:** WhatsApp Business + botón nativo; redes como adquisición hacia la tienda.
- **SEO/publicación:** procedimiento reusable en `docs/playbook/04-seo-y-publicacion.md`.
- **Comparación general de plataformas:** `docs/research/platforms-pricing-seo.md`.
- **Shortlist, matriz y condiciones de descarte:** `docs/research/shortlist-plataformas.md`.

## Frontier

### Grilling — #6 Definir operación diaria de catálogo, stock y despacho
Estado: **handoff a Camila**.

### Grilling — #7 Definir catálogo, variantes y política de stock
Estado: **handoff a Camila**.

### Grilling — #13 Confirmar titularidad, facturación y accesos con Camila
Estado: **handoff a Camila**.

### Research / validación práctica — #17 Evaluar DonWeb SitioSimple
Research documental completado. Falta validar en prueba real facilidad para operador no técnico, checkout, pagos, envíos, analytics, portabilidad, reintegros y administración de pedidos.

## Blocked

- #8 — Cambios, devoluciones y logística inversa — blocked by #6 y #7.
- #9 — Elegir plataforma del MVP — blocked by #6, #7, #8, #13 y #17. **Todavía no decidida**. La decisión debe limitarse a Tiendanube, DonWeb o Empretienda salvo evidencia nueva. Requiere aprobación explícita de `@JonatanGarbuyo`.
- #10 — Modelo comercial del servicio — blocked by #6 y #9.
- #15 — Completar playbook operativo — blocked by #6, #7, #8, #9 y #13.

## Closed research / tasks

- #2 — Comparar plataformas no-code.
- #3 — Pagos y costo efectivo.
- #4 — Logística nacional y seguro.
- #5 — Atribución y métricas.
- #11 — Arrepentimiento/devolución legal.
- #12 — Facturación y titularidad.
- #14 — WhatsApp Business y redes.
- #16 — Free tiers, planes y SEO.
- #18 — Publicar playbook en GitHub Wiki — cerrado como `not planned`; se usa Markdown navegable mediante `docs/INDEX.md`.

## Not yet specified

- Packaging y rutina concreta de despacho.
- Prototipo visual del storefront una vez elegida la plataforma.
- Criterio concreto para pasar a dominio propio/plan pago.
- Umbral de volumen que justificaría automatización.
- Qué partes del playbook se repiten para otro rubro.

## Out of scope

- E-commerce custom ahora.
- SaaS multi-tenant ahora.
- Automatizaciones complejas antes de validar volumen y dolor operativo.
