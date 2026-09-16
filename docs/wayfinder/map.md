# Wayfinder map — Tienda online nacional de bajo costo para Camila

## Destination

Llegar a una especificación de MVP y un plan de lanzamiento suficientemente claros para que Camila pueda crear y administrar una tienda online en Argentina, vendiendo a todo el país con el menor costo fijo razonable, con catálogo, checkout/pago online, logística con cobertura/seguro, atención por WhatsApp, SEO/publicación y medición de adquisición/conversión.

El resultado de este mapa es **decisión y especificación, no implementación productiva**.

## Notes

- Primer caso real: negocio existente de **ropa**.
- El MVP será **no-code**; no desarrollar software propio mientras una solución administrada cubra razonablemente el problema.
- Camila será la **responsable operativa** y administrará la tienda online.
- Jonatan aporta tecnología/desarrollo; los procesos del negocio que no conoce deben relevarse con Camila, no inferirse.
- La venta principal será **autoservicio end-to-end**; WhatsApp será asistencia, no el checkout principal.
- La atención de WhatsApp será humana en el MVP.
- El catálogo/stock puede comenzar con administración manual; no se busca sincronización compleja inicialmente.
- Prioridad: costo fijo nulo o bajo, pero evaluando costo total real por venta y carga operativa.
- Se acepta un subdominio gratuito durante la validación; **dominio propio es nice-to-have**, no requisito de lanzamiento.
- Requeridos: catálogo, links desde Facebook/Instagram, pago online, envíos/seguros, WhatsApp.
- Nice to have: dominio propio, catálogo/shop en WhatsApp, métricas, observabilidad y atribución de links/referidos.
- El repo es también base de conocimiento. El manual operativo reusable vive en `docs/playbook/`.
- Posible oportunidad futura: ofrecer el mismo servicio a otros comercios. No diseñar ahora un SaaS/plataforma genérica; separar aprendizaje reusable de restricciones específicas de indumentaria.
- Investigación con fuentes primarias y condiciones vigentes para Argentina.
- Los tickets #6, #7 y #13 quedan como handoff para que Camila los resuelva desde su chat dentro del Project.

## Decisions / research so far

- **MVP no-code:** la primera versión se arma con herramientas administradas; software custom queda fuera del destino actual.
- **Venta autoservicio principal:** catálogo → carrito → pago → envío debe funcionar sin intervención humana; WhatsApp queda como asistencia.
- **Catálogo inicialmente manual:** no exigir sincronización automática de stock/precios para validar el canal.
- **Vertical inicial ropa, playbook potencialmente reusable:** resolver el caso Camila primero y documentar qué decisiones generalizan.
- **Pagos orientados a costo/conversión:** permitir tarjeta y favorecer transferencia cuando sea razonable.
- **Atención humana por WhatsApp:** bots/IA quedan para una futura necesidad de escala.
- **Subdominio aceptable para validación / dominio propio nice-to-have:** el dominio propio no bloquea el MVP.
- **#2 Plataformas:** Tiendanube Inicial queda como baseline a validar por costo fijo $0; Empretienda como fallback si una restricción concreta bloquea el caso; social-first queda como canal auxiliar.
- **#3 Pagos:** Pago Nube cubre el MVP; tarjeta/débito/MODO + transferencia integrados. 14 días orienta a menor costo si el flujo de caja lo tolera; 7 días si hace falta liquidez más rápida.
- **#4 Logística:** Andreani/Envío Nube cubre el MVP nacional de ropa. El plan Inicial no incluye logística reversa; cambios/devoluciones requieren flujo separado.
- **#5 Medición:** UTMs + GA4 nativo + Meta Pixel/CAPI cubren la medición inicial sin costo fijo adicional.
- **#11 Consumo/devoluciones:** las ventas a distancia tienen derecho de arrepentimiento y el costo de devolución legal puede recaer en el vendedor. Verificar antes del lanzamiento la implementación vigente del botón de arrepentimiento.
- **#12 Facturación/titularidad:** el canal online debe entrar al circuito fiscal del comercio. Propuesta no aprobada: tienda/cobros/facturación a nombre del comercio; Camila administra el canal y cobra su servicio por separado. El plan Inicial no ofrece permisos diferenciados entre administradores.
- **#14 WhatsApp/redes:** WhatsApp Business + botón nativo cubren atención humana; el catálogo puede sincronizarse vía Meta Business Suite. Facebook/Instagram Shopping no están disponibles en Argentina, por lo que redes funcionan como adquisición hacia la tienda.
- **#16 Free tiers/SEO:** Tiendanube Inicial es la opción local-first con free tier permanente más fuerte. Empretienda tiene 15 días gratis y luego $10.490 ARS/mes. Odoo One App Free es $0 pero con mayor riesgo de complejidad/localización. Shopify, Wix y Ecwid requieren pago para un e-commerce transaccional permanente. Ver `docs/research/platforms-pricing-seo.md`.
- **SEO/publicación:** el proveedor resuelve parte del SEO técnico; el operador debe trabajar contenido original, títulos, descripciones, categorías, URLs, imágenes/alt, páginas informativas, Search Console/sitemap y UTMs. Criterios base en `docs/playbook/README.md`.

## Frontier

### Grilling — [Definir operación diaria de catálogo, stock y despacho](https://github.com/JonatanGarbuyo/camila-online/issues/6)
**Question:** ¿Cómo se administran hoy productos, precios y stock; con qué frecuencia cambian; quién prepara/despacha pedidos; y cuánto trabajo manual diario es aceptable para Camila?

Estado: **handoff a Camila**.

### Grilling — [Definir catálogo, variantes y política de stock](https://github.com/JonatanGarbuyo/camila-online/issues/7)
**Question:** ¿Cuántos productos/SKUs y variantes maneja el negocio, cómo se representan talles y colores, y qué política debe aplicarse ante stock bajo o agotado?

Estado: **handoff a Camila**.

### Grilling — [Confirmar titularidad, facturación y accesos con Camila](https://github.com/JonatanGarbuyo/camila-online/issues/13)
**Question:** ¿Cómo está organizado hoy el vendedor legal/facturación y qué esquema de acceso puede usar Camila?

Estado: **handoff a Camila**.

## Blocked

- [Definir cambios, devoluciones y logística inversa](https://github.com/JonatanGarbuyo/camila-online/issues/8) — blocked by #6 y #7.
- [Elegir plataforma del MVP](https://github.com/JonatanGarbuyo/camila-online/issues/9) — blocked by #6, #7, #8 y #13. **La plataforma todavía no está decidida.** Tiendanube Inicial es baseline, no decisión final. Requiere aprobación explícita de `@JonatanGarbuyo`.
- [Definir modelo comercial del servicio de administración](https://github.com/JonatanGarbuyo/camila-online/issues/10) — blocked by #6 y #9. Hipótesis: el comercio paga costos directos; Camila puede cobrar fee de administración y eventualmente comisión por ventas.
- [Completar playbook para levantar y administrar la tienda](https://github.com/JonatanGarbuyo/camila-online/issues/15) — blocked by #6, #7, #8, #9 y #13. Skeleton en `docs/playbook/README.md`.

## Closed research

- #2 — Comparar plataformas no-code.
- #3 — Evaluar pagos y costo efectivo.
- #4 — Validar logística nacional y seguro.
- #5 — Definir atribución y métricas mínimas.
- #11 — Obligaciones legales de arrepentimiento/devolución.
- #12 — Facturación y titularidad del canal online.
- #14 — WhatsApp Business y canales sociales.
- #16 — Free tiers, planes y SEO.

## Not yet specified

- Packaging y rutina concreta de despacho.
- Prototipo visual del storefront una vez elegida la plataforma.
- Criterio concreto para pasar de subdominio a dominio propio/plan pago.
- Umbral de volumen que justificaría automatización de WhatsApp, stock o reporting.
- Qué partes del playbook podrían repetirse para un segundo comercio de otro rubro.

## Out of scope

- Construir ahora una plataforma e-commerce custom.
- Construir un SaaS multi-tenant para comercios.
- Reemplazar procesos internos que no sean necesarios para habilitar el canal online.
- Automatizaciones complejas antes de comprobar volumen y dolor operativo.