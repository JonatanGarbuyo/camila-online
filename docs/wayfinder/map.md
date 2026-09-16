# Wayfinder map — Tienda online nacional de bajo costo para Camila

## Destination

Llegar a una especificación de MVP y un plan de lanzamiento suficientemente claros para que Camila pueda crear y administrar una tienda online en Argentina, vendiendo a todo el país con el menor costo fijo razonable, con catálogo, checkout/pago online, logística con cobertura/seguro, atención por WhatsApp y medición de adquisición/conversión.

El resultado de este mapa es **decisión y especificación, no implementación productiva**.

## Notes

- Primer caso real: negocio existente de **ropa**.
- El MVP será **no-code**; no desarrollar software propio mientras una solución administrada cubra razonablemente el problema.
- La venta principal será **autoservicio end-to-end**; WhatsApp será asistencia, no el checkout principal.
- La atención de WhatsApp será humana en el MVP.
- El catálogo/stock puede comenzar con administración manual; no se busca sincronización compleja inicialmente.
- Prioridad: costo fijo nulo o bajo, pero evaluando costo total real por venta y carga operativa.
- Se acepta un subdominio gratuito durante la validación; dominio propio no es requisito de lanzamiento.
- Requeridos: catálogo, links desde Facebook/Instagram, pago online, envíos/seguros, WhatsApp.
- Nice to have: catálogo/shop en WhatsApp, métricas, observabilidad y atribución de links/referidos.
- Posible oportunidad futura: ofrecer el mismo servicio a otros comercios. No diseñar ahora un SaaS/plataforma genérica; separar aprendizaje reusable de restricciones específicas de indumentaria.
- Investigación con fuentes primarias y condiciones vigentes para Argentina.

## Decisions so far

- **MVP no-code:** la primera versión se arma con herramientas administradas; software custom queda fuera del destino actual.
- **Venta autoservicio principal:** catálogo → carrito → pago → envío debe funcionar sin intervención humana; WhatsApp queda como asistencia.
- **Catálogo inicialmente manual:** no exigir sincronización automática de stock/precios para validar el canal.
- **Vertical inicial ropa, playbook potencialmente reusable:** resolver el caso Camila primero y documentar qué decisiones generalizan.
- **Pagos orientados a costo/conversión:** permitir tarjeta y favorecer transferencia cuando sea razonable.
- **Atención humana por WhatsApp:** bots/IA quedan para una futura necesidad de escala.
- **Subdominio aceptable para validación:** dominio propio no bloquea el MVP.

## Frontier

### Research — Comparar plataformas no-code de bajo/nulo costo
**Question:** ¿Qué plataforma cubre mejor el MVP de Camila con el menor costo total y menor carga operativa?

Candidatas iniciales:
1. Tiendanube Inicial.
2. Empretienda.
3. Social-first: WhatsApp Business + Mercado Pago Link + logística manual.

Estado: investigación inicial en `docs/research/options.md`.

### Research — Validar logística para indumentaria
**Question:** ¿Andreani mediante Tiendanube Inicial cubre bien el flujo nacional de ropa y qué costos/condiciones de seguro importan?

Estado: investigación inicial en `docs/research/shipping-insurance.md`.

### Research — Diseñar atribución mínima viable
**Question:** ¿Qué combinación mínima permite medir clicks, fuente/campaña, checkout y ventas sin sumar costo fijo?

Estado: propuesta inicial en `docs/research/measurement.md`.

### Grilling — Definir operación diaria de Camila
**Question:** ¿Quién mantiene productos, precios y stock; con qué frecuencia cambia; cómo prepara/despacha pedidos; y cuánto trabajo manual diario es aceptable?

Bloquea: decisión final de plataforma y playbook operativo.

### Grilling — Definir restricciones físicas del catálogo
**Question:** ¿Cuántos SKUs/variantes hay aproximadamente, cómo se manejan talles/colores y qué volumen de pedidos sería éxito en la primera etapa?

Bloquea: validación práctica de carga de catálogo y operación.

## Not yet specified

- Flujo de cambios/devoluciones, especialmente cambios de talle.
- Política de stock agotado y reservas.
- Packaging y proceso de despacho.
- Prototipo visual del storefront una vez elegida la plataforma.
- Facturación fiscal/ARCA y automatización contable según situación del negocio.
- Criterio concreto para pasar de subdominio a dominio propio/plan pago.
- Umbral de volumen que justificaría automatización de WhatsApp, stock o reporting.
- Qué partes del playbook podrían repetirse para un segundo comercio de otro rubro.

## Out of scope

- Construir ahora una plataforma e-commerce custom.
- Construir un SaaS multi-tenant para comercios.
- Reemplazar procesos internos que no sean necesarios para habilitar el canal online.
- Automatizaciones complejas antes de comprobar volumen y dolor operativo.
