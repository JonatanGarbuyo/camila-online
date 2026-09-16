# Wayfinder map — Tienda online nacional de bajo costo para Camila

## Destination

Llegar a una especificación de MVP y un plan de lanzamiento suficientemente claros para que Camila pueda crear y administrar una tienda online en Argentina, vendiendo a todo el país con el menor costo fijo razonable, con catálogo, checkout/pago online, logística con cobertura/seguro, atención por WhatsApp y medición de adquisición/conversión.

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
- Se acepta un subdominio gratuito durante la validación; dominio propio no es requisito de lanzamiento.
- Posible oportunidad futura: ofrecer el mismo servicio a otros comercios. No diseñar ahora un SaaS/plataforma genérica; separar aprendizaje reusable de restricciones específicas de indumentaria.
- Los tickets #6, #7 y #13 son handoff a Camila porque requieren conocimiento real del negocio.

## Decisions / research so far

- **MVP no-code:** la primera versión se arma con herramientas administradas; software custom queda fuera del destino actual.
- **Venta autoservicio principal:** catálogo → carrito → pago → envío debe funcionar sin intervención humana; WhatsApp queda como asistencia.
- **Catálogo inicialmente manual:** no exigir sincronización automática de stock/precios para validar el canal.
- **Vertical inicial ropa, playbook potencialmente reusable:** resolver el caso Camila primero y documentar qué decisiones generalizan.
- **Pagos orientados a costo/conversión:** permitir tarjeta y favorecer transferencia cuando sea razonable.
- **Atención humana por WhatsApp:** bots/IA quedan para una futura necesidad de escala.
- **Subdominio aceptable para validación:** dominio propio no bloquea el MVP.
- **[#2 Plataformas](https://github.com/JonatanGarbuyo/camila-online/issues/2):** Tiendanube Inicial es la baseline a validar por costo fijo $0; Empretienda es fallback si aparece una restricción concreta; social-first queda como canal auxiliar.
- **[#3 Pagos](https://github.com/JonatanGarbuyo/camila-online/issues/3):** Pago Nube cubre el MVP; tarjeta/débito/MODO + transferencia integrados. Propuesta reversible: 14 días si se prioriza costo y el flujo de caja lo tolera; 7 días si hace falta liquidez más rápida.
- **[#4 Logística](https://github.com/JonatanGarbuyo/camila-online/issues/4):** Andreani/Envío Nube cubre el MVP nacional de ropa. El plan Inicial no incluye logística reversa; cambios/devoluciones requieren flujo separado.
- **[#5 Medición](https://github.com/JonatanGarbuyo/camila-online/issues/5):** UTMs + GA4 nativo + Meta Pixel/CAPI cubren la medición inicial sin costo fijo adicional.
- **[#11 Consumo y devoluciones](https://github.com/JonatanGarbuyo/camila-online/issues/11):** las ventas a distancia tienen derecho de arrepentimiento; los costos de la devolución legal pueden recaer en el vendedor. Tiendanube incluye flujo de arrepentimiento, pero hay que verificar antes del lanzamiento su implementación respecto de la Disposición 954/2025. Ver `docs/research/legal-consumer.md`.
- **[#12 Facturación y titularidad](https://github.com/JonatanGarbuyo/camila-online/issues/12):** el canal online debe entrar al circuito fiscal del comercio. Propuesta no aprobada: tienda/cobros/facturación a nombre del comercio; Camila administra el canal y cobra su servicio por separado. El plan Inicial no ofrece permisos diferenciados entre administradores. Ver `docs/research/fiscal-invoicing.md`.
- **[#14 WhatsApp y redes](https://github.com/JonatanGarbuyo/camila-online/issues/14):** WhatsApp Business + botón nativo cubren atención humana; el catálogo puede sincronizarse vía Meta Business Suite. Facebook/Instagram Shopping no están disponibles en Argentina, por lo que redes deben funcionar como adquisición hacia la tienda. Ver `docs/research/social-whatsapp.md`.

## Frontier

### Grilling — [#6 Definir operación diaria de catálogo, stock y despacho](https://github.com/JonatanGarbuyo/camila-online/issues/6)

Estado: **handoff a Camila**. Relevar sistema actual de stock/facturación, frecuencia de cambios, responsables y volumen manual aceptable.

### Grilling — [#7 Definir catálogo, variantes y política de stock](https://github.com/JonatanGarbuyo/camila-online/issues/7)

Estado: **handoff a Camila**. Relevar cantidad de productos/SKUs, talles/colores y política ante stock bajo o agotado.

### Grilling — [#13 Confirmar titularidad, facturación y accesos con Camila](https://github.com/JonatanGarbuyo/camila-online/issues/13)

Estado: **handoff a Camila**. Relevar quién factura hoy, qué herramienta usan y si es aceptable que el comercio sea titular de cuentas/cobros mientras Camila administra con acceso propio.

## Blocked

- [#8 Definir cambios, devoluciones y logística inversa](https://github.com/JonatanGarbuyo/camila-online/issues/8) — blocked by #6 y #7. Debe separar arrepentimiento legal de cambio comercial por talle/color.
- [#9 Elegir plataforma del MVP](https://github.com/JonatanGarbuyo/camila-online/issues/9) — blocked by #6, #7, #8 y #13. Requiere aprobación explícita de `@JonatanGarbuyo`.
- [#10 Definir modelo comercial del servicio de administración](https://github.com/JonatanGarbuyo/camila-online/issues/10) — blocked by #6 y #9. Hipótesis: comercio paga costos directos; Camila cobra fee de administración y eventualmente comisión. Valores/estructura requieren aprobación de `@JonatanGarbuyo`.

## Launch checks pendientes

- Verificar en una tienda real la ubicación/comportamiento del Botón de Arrepentimiento frente a la Disposición 954/2025.
- Validar que el esquema de acceso total de administradores del plan Inicial sea aceptable para dueños + Camila.
- Confirmar que el circuito actual de facturación pueda absorber pedidos online manualmente al comienzo.
- Diseñar packaging y rutina de despacho.
- Hacer una compra de prueba completa una vez configurada la tienda candidata.

## Not yet specified

- Prototipo visual del storefront una vez elegida la plataforma.
- Criterio concreto para pasar de subdominio a dominio propio/plan pago.
- Umbral de volumen que justificaría automatización de WhatsApp, stock o reporting.
- Qué partes del playbook podrían repetirse para un segundo comercio de otro rubro.

## Out of scope

- Construir ahora una plataforma e-commerce custom.
- Construir un SaaS multi-tenant para comercios.
- Reemplazar procesos internos que no sean necesarios para habilitar el canal online.
- Automatizaciones complejas antes de comprobar volumen y dolor operativo.
