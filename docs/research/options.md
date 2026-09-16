# Opciones de arquitectura no-code

_Verificado: 2026-09-16._

## Conclusión de research

Para el MVP de Camila, **Tiendanube Inicial queda como baseline recomendada para validar el canal**, no como decisión final de plataforma.

Motivos:

- costo fijo de plataforma: $0;
- checkout autoservicio integrado;
- catálogo sin límite publicado de productos/ventas/visitas;
- Pago Nube integrado con tarjeta, débito, MODO y transferencia;
- Andreani integrado para envíos;
- Google Analytics;
- botón de WhatsApp;
- Pixel + API de conversiones de Meta;
- operación pensada para usuarios no técnicos.

**Empretienda queda como alternativa principal** si las restricciones del plan gratuito de Tiendanube se vuelven relevantes: permite más medios de pago y envío, dominio propio, carga masiva, GA, Pixel y WhatsApp dentro de un único plan pago bajo.

**Social-first (WhatsApp Business + links de pago) no cumple como arquitectura principal** porque el flujo de carrito de WhatsApp termina en una conversación para acordar pago/entrega. Puede servir como canal auxiliar, pero contradice la decisión de venta autoservicio end-to-end.

La elección final queda pendiente de los tickets de pagos, logística, catálogo/operación y cambios/devoluciones.

---

## 1. Tiendanube Inicial — costo fijo $0

### Hechos relevantes para Argentina

- plan Inicial gratuito;
- productos, ventas y visitas sin límite publicados;
- subdominio gratuito `*.mitiendanube.com`;
- sin dominio propio en plan Inicial;
- Pago Nube como único medio de pago integrado del plan gratuito;
- Andreani como único operador integrado del plan gratuito;
- Google Analytics disponible;
- botón de WhatsApp disponible;
- Pixel y API de conversiones de Facebook/Meta disponibles;
- usuarios administradores ilimitados, todos con acceso total;
- no permite importar/exportar productos masivamente;
- no permite exportar ventas ni lista de clientes;
- solo se puede publicar la plantilla incluida; otros diseños requieren plan pago.

### Pago Nube — Plan Inicial

Tarifas publicadas al 04/08/2026:

- tarjeta/débito/MODO, dinero en 1 día: 6,40% + IVA;
- 7 días: 4,45% + IVA;
- 14 días: 3,50% + IVA;
- transferencia: 1,50% + IVA.

Las ventas cobradas con Pago Nube no pagan costo por transacción adicional de Tiendanube. La comisión se calcula sobre el total de la orden, incluyendo envío.

### Encaje

Muy fuerte para validar si:

- Andreani cubre correctamente el flujo real de ropa;
- Pago Nube es aceptable en costo y experiencia;
- la carga manual del catálogo es tolerable;
- no necesitamos exportación masiva al inicio;
- el subdominio gratuito es suficiente durante la validación.

### Restricciones que podrían forzar migración o plan pago

- necesidad de Mercado Pago u otra pasarela;
- necesidad de otro correo/logística;
- dominio propio;
- catálogo grande con mantenimiento masivo;
- exportación operativa de ventas/clientes/productos;
- permisos diferenciados entre usuarios.

Fuentes primarias:
- https://www.tiendanube.com/planes-y-precios
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube
- https://ayuda.tiendanube.com/es_AR/123482-planes/cuales-son-los-costos-del-plan-tienda-inicial
- https://ayuda.tiendanube.com/es_AR/pago-nube/cuales-son-las-comisiones-de-pago-nube

---

## 2. Empretienda — costo fijo bajo

La página oficial consultada publica:

- ARS 10.490 finales por mes;
- 15 días de prueba gratis;
- sin comisión de plataforma por venta;
- productos y ventas ilimitados;
- subdominio gratuito y dominio propio configurable;
- medios de pago: Ualá Bis, Mercado Pago, efectivo, transferencia o acordar luego de comprar;
- envíos: OCA, Correo Argentino, Andreani, E-Pick, métodos personalizados y puntos de retiro;
- importación masiva de productos;
- Google Analytics;
- Facebook Pixel;
- chat de WhatsApp;
- administración desde celular;
- soporte humano por email.

### Encaje

Es más flexible que Tiendanube Inicial desde el día uno. El costo mensual compra principalmente:

- libertad de pasarela de pago;
- libertad logística;
- dominio propio;
- operaciones masivas de catálogo;
- menor riesgo de quedar bloqueados por una sola integración.

### Trade-off

Para una tienda que todavía está validando el canal, los ARS 10.490 mensuales son un costo fijo que Tiendanube Inicial evita. Por eso Empretienda no desplaza automáticamente a Tiendanube en el MVP; se vuelve preferible cuando una restricción concreta justifica ese abono.

Fuente primaria:
- https://api.empretienda.com/

---

## 3. Social-first — WhatsApp Business + Mercado Pago Link

### Qué sí ofrece

WhatsApp Business es gratuito para pequeñas empresas y permite:

- catálogo de productos;
- colecciones;
- enlaces compartibles al catálogo/producto;
- carrito dentro de WhatsApp.

Mercado Pago permite links de pago sin costo fijo y cobra solo cuando se vende.

Tarifas publicadas de Link de Pago al 16/09/2026:

- inmediato: 6,29% + IVA;
- 10 días: 4,39% + IVA;
- 18 días: 3,39% + IVA;
- 35 días: 1,49% + IVA.

### Por qué no es el storefront principal

WhatsApp documenta que el carrito se envía al chat con la empresa para **discutir opciones de pago**. Eso deja el cierre dentro de una venta asistida, no en un checkout autoservicio.

Además:

- stock y conciliación quedan más manuales;
- cotización de envío no está unificada con el carrito;
- la atribución `visita → checkout → compra` se fragmenta;
- aumenta el riesgo de errores operativos al crecer el volumen.

### Uso recomendado

Canal auxiliar para:

- consultas de talle/producto;
- recuperación de clientes;
- compartir productos;
- ventas excepcionales asistidas.

No usar como arquitectura principal mientras siga vigente la decisión de autoservicio end-to-end.

Fuentes primarias:
- https://faq.whatsapp.com/es/26000275/
- https://faq.whatsapp.com/1312962072846852/
- https://www.mercadopago.com.ar/herramientas-para-vender/link-de-pago

---

## 4. Storefront custom / headless

Fuera del destino actual.

Aunque el hosting podría ser barato, traslada el costo a desarrollo, mantenimiento, seguridad, integraciones y soporte. Solo reconsiderar si una restricción concreta descarta las plataformas administradas.

---

## Regla de decisión derivada

1. Validar primero si **Tiendanube Inicial** pasa los tickets de logística, pagos y operación.
2. Si falla por una restricción concreta, evaluar **Empretienda** como fallback antes de considerar desarrollo propio.
3. Mantener **WhatsApp Business** como canal de asistencia y catálogo auxiliar, no como checkout principal.
