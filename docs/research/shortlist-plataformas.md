# Shortlist de plataformas para el MVP

_Estado: shortlist reducida por decisión del owner. La plataforma final todavía no está decidida._

_Verificado documentalmente: 2026-09-16. La prueba práctica todavía está pendiente._

## Plataformas activas

1. **Tiendanube**
2. **DonWeb SitioSimple**

## Plataforma descartada en esta etapa

### Empretienda

Empretienda sale de la evaluación activa.

No se descarta porque no pueda cobrar: permite integrar medios de pago de terceros como Mercado Pago, Ualá Bis y transferencia.

Se descarta frente a Tiendanube y DonWeb porque, para este proyecto:

- la documentación pública disponible es bastante menos completa;
- no presenta una pasarela propia/integrada comparable a Pago Nube;
- depende de proveedores externos para pagos;
- sigue poco claro el modelo de usuarios/permisos para que Camila administre sin compartir credenciales;
- Tiendanube y DonWeb ofrecen hoy una propuesta más clara para comparar operación, costos y soporte.

Puede reabrirse solo si las dos finalistas fallan por una restricción concreta.

## Objetivo

Elegir entre Tiendanube y DonWeb la opción más simple para que Camila administre la tienda con baja carga operativa, buen encaje con Argentina y costo total razonable.

## Regla de fragmentación

La fragmentación se evalúa por **tipo de tarea**, no por proveedor.

### Pagos

Puede ser aceptable que cobros, conciliación, devoluciones o reintegros se operen en un panel separado del panel principal de la tienda si Camila y el comercio consideran razonable ese flujo.

Lo que se evalúa es la carga operativa de cambiar de sistema y mantener trazabilidad.

### Envíos

Es una desventaja fuerte que la operación normal obligue a entrar habitualmente en otro panel para generar o pagar etiquetas, preparar despachos, consultar tracking, cancelar envíos o resolver incidencias.

Preferir logística integrada o un flujo externo tan directo que no agregue trabajo cotidiano relevante.

## Lectura preliminar

### Tiendanube Inicial

Fortalezas:

- costo fijo $0;
- pago y logística muy integrados;
- operación local orientada a Argentina.

Restricciones:

- sin dominio propio en Inicial;
- sin carga/exportación masiva;
- Pago Nube como pago integrado;
- Andreani/Envío Nube como logística integrada;
- usuarios adicionales con acceso total.

### DonWeb SitioSimple

Fortalezas:

- costo fijo muy bajo;
- dominio propio;
- carga/edición masiva;
- varios medios de pago y envío;
- usuarios con permisos diferenciados;
- modelo futuro de revendedores/partners.

Riesgo principal:

- validar que pagos y, especialmente, envíos no fragmenten demasiado la operación diaria.

## Condiciones de descarte

### Tiendanube Inicial deja de ser suficiente si…

- el catálogo hace inviable la carga manual;
- se necesita dominio propio desde el inicio;
- Pago Nube o Andreani no sirven para la operación real;
- se necesitan exportaciones/acciones masivas frecuentes;
- los dueños no aceptan acceso total para Camila.

### DonWeb deja de ser suficiente si…

- el panel resulta confuso para Camila;
- la fragmentación de pagos supera lo que Camila/comercio consideran razonable;
- la logística obliga habitualmente a operar otro panel para etiquetas, despacho o tracking;
- analytics/atribución son insuficientes;
- el checkout móvil tiene fricción material.

## Prueba práctica

Las cuentas y pruebas se ejecutarán manualmente por Camila o Jonatan siguiendo `docs/research/protocolo-prueba-plataformas.md`.

La prueba activa compara solamente **Tiendanube y DonWeb**.

No usar credenciales, cuentas sensibles ni medios de pago reales en GitHub.

La decisión final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.
