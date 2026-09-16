# Opciones iniciales de arquitectura no-code

_Verificado originalmente: 2026-09-16. Ver también `platforms-pricing-seo.md` para comparación ampliada y precios/SEO actuales._

## 1. Tiendanube Inicial — costo fijo $0

Hechos relevantes para Argentina:

- plan Inicial gratuito, sin costo mensual;
- productos cargables manualmente sin límite indicado por la documentación del plan;
- dominio gratuito `*.mitiendanube.com`, sin dominio propio en el plan Inicial;
- Pago Nube como único medio de pago integrado en el plan gratuito;
- Andreani como único medio de envío integrado en el plan gratuito;
- Google Analytics disponible;
- botón de WhatsApp disponible;
- Pixel y API de conversiones de Facebook disponibles;
- no permite importación/exportación masiva de productos en el plan Inicial.

### Encaje

Muy fuerte para el MVP si:

- Andreani cubre correctamente la logística de ropa;
- Pago Nube resulta aceptable en costo/medios de pago;
- el subdominio de Tiendanube es aceptable durante validación;
- se prioriza que Camila administre la tienda sin soporte técnico.

### Riesgo

Costo fijo cero no significa costo total cero. Hay que medir comisión de cobro, costo logístico, seguro, packaging y carga operativa.

Fuentes primarias:
- https://ayuda.tiendanube.com/es_AR/123482-planes/cuales-son-los-costos-del-plan-tienda-inicial
- https://ayuda.tiendanube.com/es_AR/123482-planes/que-funcionalidades-incluye-el-plan-gratuito-de-tiendanube
- https://ayuda.tiendanube.com/es_AR/123482-planes/en-que-planes-puedo-instalar-aplicaciones-en-mi-tiendanube

## 2. Empretienda — costo fijo bajo

La página oficial consultada publica:

- ARS 10.490 finales por mes;
- 15 días de prueba;
- sin comisión de plataforma por venta;
- productos físicos y digitales;
- administración orientada a usuarios no técnicos;
- dominio gratuito y posibilidad de dominio propio;
- múltiples pagos/envíos, carga masiva, GA, Pixel y SEO automático.

### Encaje

Alternativa importante si un abono bajo evita restricciones del plan gratuito de Tiendanube y reduce el costo/operación total.

Fuente primaria:
- https://api.empretienda.com/

## 3. Odoo Online One App Free — alternativa gratuita secundaria

Odoo publica un plan One App Free de US$0 con usuarios ilimitados y Odoo Online. Si eCommerce depende de Website/Invoicing, las dependencias se incluyen sin costo adicional según su pricing.

Tiene capacidades SEO técnicas fuertes, pero no es actualmente la baseline porque el encaje de pagos/logística/operación para Argentina puede requerir más configuración que Tiendanube o Empretienda.

Fuentes:
- https://www.odoo.com/pricing
- https://www.odoo.com/documentation/19.0/applications/websites/website/structure/seo.html

## 4. Social-first — costo fijo casi cero

Stack conceptual:

- WhatsApp Business como conversación/catálogo auxiliar;
- Mercado Pago Link de Pago;
- despacho gestionado manualmente;
- registro simple de pedidos y origen de campaña.

### Ventajas

- prácticamente sin costo fijo;
- útil para validar demanda con muy pocos productos;
- aprovecha canales sociales existentes.

### Costos ocultos

- conciliación y stock manuales;
- checkout fragmentado;
- cotización/selección de envío menos integrada;
- atribución de ventas más difícil;
- más dependencia de disciplina operativa.

Por la decisión de venta autoservicio end-to-end, queda como canal auxiliar, no arquitectura principal.

## 5. Otras plataformas evaluadas

- Shopify: prueba/promoción inicial, pero luego costo fijo en USD; no free tier permanente.
- Wix: puede publicarse sitio gratuito, pero e-commerce con pagos requiere upgrade.
- Ecwid: planes pagos; Starter no debe tratarse como free tier permanente.

Ver detalle en `docs/research/platforms-pricing-seo.md`.

## 6. Storefront custom / headless

Fuera del destino actual.

Aunque el hosting podría ser barato, traslada el costo a desarrollo, mantenimiento, seguridad, integraciones y soporte. Solo reconsiderar si una restricción concreta descarta las plataformas administradas.

## Hipótesis de trabajo

**Tiendanube Inicial sigue siendo la baseline a vencer, no una decisión final.** La elección formal vive en #9 y depende de los relevamientos pendientes con Camila.