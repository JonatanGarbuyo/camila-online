# Shortlist de plataformas para el MVP

_Estado: shortlist acordada para evaluación. No es todavía la decisión final de plataforma._

_Verificado documentalmente: 2026-09-16. La prueba práctica todavía está pendiente._

## Plataformas activas

1. **Tiendanube**
2. **DonWeb SitioSimple**
3. **Empretienda**

Shopify, Wix, Odoo y otras alternativas quedan fuera de la evaluación activa salvo que aparezca una restricción nueva que invalide las tres opciones anteriores.

## Objetivo

Elegir la plataforma más simple para que Camila pueda administrar la tienda con baja carga operativa, buen encaje con Argentina y costo total razonable.

## Regla de fragmentación

La fragmentación se evalúa por **tipo de tarea**, no por proveedor.

### Pagos

Puede ser aceptable que cobros, conciliación, devoluciones o reintegros se operen en un panel de pago separado del panel principal de la tienda **si Camila y el comercio consideran razonable ese flujo**.

No importa si el proveedor es Mercado Pago, Pago Nube, Mobbex, Ualá u otro: lo que se evalúa es la carga operativa de cambiar de sistema y mantener trazabilidad.

### Envíos

Es una desventaja fuerte que la operación normal obligue a entrar habitualmente en otro panel para:

- generar o pagar etiquetas;
- preparar despachos;
- consultar tracking;
- cancelar envíos;
- resolver incidencias.

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

### Empretienda

Fortalezas:

- un único plan local simple;
- carga masiva;
- varios pagos/envíos;
- dominio propio;
- Analytics/Pixel/Shopping publicados.

Pendiente crítico:

- verificar acceso delegado/multiusuario seguro sin compartir contraseña.

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

### Empretienda deja de ser suficiente si…

- no permite accesos separados y seguros;
- obliga a compartir contraseña;
- la fragmentación de pagos o envíos resulta operativamente incómoda;
- SEO, portabilidad o reporting no alcanzan el procedimiento requerido.

## Prueba práctica

Las cuentas y pruebas se ejecutarán manualmente por Camila o Jonatan siguiendo `docs/research/protocolo-prueba-plataformas.md`.

No usar credenciales, cuentas sensibles ni medios de pago reales en GitHub.

La decisión final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.
