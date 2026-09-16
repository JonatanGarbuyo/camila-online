# Opciones iniciales de arquitectura no-code

_Verificado: 2026-09-16._

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
- administración orientada a usuarios no técnicos.

### Encaje

Alternativa importante si un abono bajo evita restricciones del plan gratuito de Tiendanube y reduce el costo/operación total.

### Pendiente de validar en prueba

- medios de pago concretos y sus costos;
- logística nacional;
- tracking/analytics;
- exportación de pedidos/clientes;
- dominio propio;
- integración de WhatsApp;
- manejo de variantes de ropa.

Fuente primaria:
- https://api.empretienda.com/

## 3. Social-first — costo fijo casi cero

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

Mercado Pago confirma que Link de Pago puede compartirse por WhatsApp, Instagram y Facebook y que no requiere e-commerce.

Fuente primaria:
- https://www.mercadopago.com.ar/herramientas-para-vender/link-de-pago

## 4. Storefront custom / headless

Fuera del destino actual.

Aunque el hosting podría ser barato, traslada el costo a desarrollo, mantenimiento, seguridad, integraciones y soporte. Solo reconsiderar si una restricción concreta descarta las plataformas administradas.

## Hipótesis de trabajo

**Tiendanube Inicial es actualmente la baseline a vencer**, no una decisión final. Es la candidata que mejor combina costo fijo cero, checkout integrado, operación no-code, WhatsApp y medición sin construir software.
