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
- **[Comparar plataformas no-code para el MVP](https://github.com/JonatanGarbuyo/camila-online/issues/2):** Tiendanube Inicial queda como baseline a validar por costo fijo $0; Empretienda como fallback si una restricción concreta bloquea el caso; WhatsApp Business + links de pago queda como canal auxiliar, no storefront principal.

## Frontier

### Research — [Evaluar pagos y costo efectivo por venta](https://github.com/JonatanGarbuyo/camila-online/issues/3)
**Question:** ¿Qué combinación de medios de pago y plazo de acreditación conviene para el MVP, considerando costo efectivo, conversión, cuotas, conciliación y operación?

Estado: investigación inicial en `docs/research/payments.md`.

### Research — [Validar logística nacional y seguro para indumentaria](https://github.com/JonatanGarbuyo/camila-online/issues/4)
**Question:** ¿Andreani mediante el plan Inicial cubre correctamente el MVP de indumentaria para envíos nacionales, y qué política de seguro/cobertura conviene?

Estado: investigación inicial en `docs/research/shipping-insurance.md`.

### Research — [Definir atribución y métricas mínimas](https://github.com/JonatanGarbuyo/camila-online/issues/5)
**Question:** ¿Qué medición mínima permite atribuir visitas y ventas a Instagram, Facebook, WhatsApp y referidos sin sumar costo fijo ni complejidad innecesaria?

Estado: propuesta inicial en `docs/research/measurement.md`.

### Grilling — [Definir operación diaria de catálogo, stock y despacho](https://github.com/JonatanGarbuyo/camila-online/issues/6)
**Question:** ¿Cómo se administran hoy productos, precios y stock; con qué frecuencia cambian; quién prepara/despacha pedidos; y cuánto trabajo manual diario es aceptable para Camila?

### Grilling — [Definir catálogo, variantes y política de stock](https://github.com/JonatanGarbuyo/camila-online/issues/7)
**Question:** ¿Cuántos productos/SKUs y variantes maneja el negocio, cómo se representan talles y colores, y qué política debe aplicarse ante stock bajo o agotado?

## Blocked

- [Definir cambios, devoluciones y logística inversa](https://github.com/JonatanGarbuyo/camila-online/issues/8) — blocked by #6 y #7.
- [Elegir plataforma del MVP](https://github.com/JonatanGarbuyo/camila-online/issues/9) — blocked by #3, #4, #5, #6, #7 y #8. Esta es la decisión final y requerirá aprobación explícita de `@JonatanGarbuyo`.

## Not yet specified

- Packaging y proceso de despacho, hasta conocer la operación actual.
- Facturación fiscal/ARCA y automatización contable según situación del negocio.
- Prototipo visual del storefront una vez elegida la plataforma.
- Criterio concreto para pasar de subdominio a dominio propio/plan pago.
- Umbral de volumen que justificaría automatización de WhatsApp, stock o reporting.
- Qué partes del playbook podrían repetirse para un segundo comercio de otro rubro.

## Out of scope

- Construir ahora una plataforma e-commerce custom.
- Construir un SaaS multi-tenant para comercios.
- Reemplazar procesos internos que no sean necesarios para habilitar el canal online.
- Automatizaciones complejas antes de comprobar volumen y dolor operativo.
