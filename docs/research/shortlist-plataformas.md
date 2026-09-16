# Shortlist de plataformas para el MVP

_Estado: tres finalistas para prueba manual. No es la decisión final._

## Finalistas

1. **Tiendanube**
2. **DonWeb SitioSimple**
3. **Empretienda**

La comparación debe premiar la **menor complejidad suficiente** para que Camila administre la tienda correctamente, no la plataforma con más funciones.

## Matriz resumida

| Tema | Tiendanube Inicial | DonWeb SitioSimple | Empretienda |
| --- | --- | --- | --- |
| Costo fijo publicado | $0 | ~$3.900/mes equivalente en anual | $10.490/mes |
| Pago | Pago Nube integrado | Mercado Pago / Mobbex / otros | Mercado Pago / Ualá / otros |
| Envíos | Andreani/Envío Nube muy integrado | Andreani, OCA, Envia.com y otros | Varias opciones locales |
| Dominio propio | No en Inicial | Sí | Sí |
| Carga masiva | No en Inicial | Sí | Sí |
| Accesos | Varios usuarios, todos con acceso total en Inicial | Usuarios con permisos por secciones | Pendiente de verificar acceso delegado |
| SEO/publicación | Bueno | Bueno | Bueno sobre papel; validar controles finos |
| Principal ventaja | Costo $0 + operación centralizada | Bajo costo + flexibilidad + permisos | Simplicidad local en un único plan |
| Principal riesgo | Restricciones del plan gratis | Fragmentación entre paneles externos | Accesos/permisos y profundidad de integraciones |

## Regla clave: no toda fragmentación pesa igual

### Fragmentación de pagos

Puede ser **aceptable** operar Mercado Pago por separado cuando:

- el comercio ya tiene cuenta de Mercado Pago;
- desea conservar esa misma cuenta;
- Camila considera razonable entrar allí para conciliación, reintegros o incidencias;
- la tienda recibe correctamente el estado del pedido/pago y no exige conciliación manual riesgosa.

Por lo tanto, que DonWeb use Mercado Pago externo **no es por sí solo motivo de descarte**.

### Fragmentación de envíos

Es una **desventaja fuerte** si para cada pedido Camila debe entrar habitualmente a otro panel para:

- generar o pagar etiquetas;
- preparar el despacho;
- obtener tracking;
- actualizar estados;
- resolver incidencias.

Preferimos que el flujo `pedido → etiqueta → despacho → seguimiento` quede dentro de la tienda o sea muy directo.

Esta diferencia debe ponderarse más que la simple cantidad de proveedores de envío disponibles.

## Cómo puede inclinarse la decisión

### DonWeb gana peso si…

- el comercio ya usa Mercado Pago y quiere conservarlo;
- Camila acepta esa separación para pagos;
- el flujo de envíos resulta integrado/directo en la prueba;
- los permisos separados comercio/Camila funcionan bien;
- la operación diaria sigue siendo simple pese a usar proveedores externos.

### Tiendanube gana peso si…

- Camila valora fuertemente operar pagos, pedidos y logística desde un mismo ecosistema;
- Andreani sirve para el comercio;
- el catálogo inicial puede mantenerse manualmente;
- no hace falta dominio propio al lanzamiento;
- los dueños aceptan el esquema de accesos del plan Inicial.

### Empretienda gana peso si…

- su panel resulta el más simple para Camila;
- confirma acceso separado legítimo para administradora y comercio;
- pagos y envíos quedan suficientemente centralizados;
- la diferencia de costo fijo se compensa con menos carga operativa.

## Condiciones de descarte

### Tiendanube Inicial

Deja de ser suficiente si la carga manual de catálogo/stock es inviable, Andreani no sirve, Pago Nube no encaja, los accesos totales no son aceptables o el upgrade necesario hace perder su ventaja económica.

### DonWeb

Deja de ser suficiente si el flujo normal obliga a alternar continuamente entre tienda, pago y logística, especialmente si **envíos** requieren operación cotidiana en un segundo panel.

### Empretienda

Deja de ser suficiente si obliga a compartir contraseña, si no ofrece acceso delegado adecuado o si pagos/envíos requieren más trabajo manual del esperado.

## Prueba manual

Camila o Jonatan crearán manualmente las cuentas de prueba y usarán:

[`protocolo-prueba-plataformas.md`](protocolo-prueba-plataformas.md)

No automatizar altas ni guardar credenciales reales en el repo.

## Resultado esperado

La decisión final debe poder explicarse con restricciones concretas observadas durante la prueba y con las respuestas de Camila sobre operación diaria y tolerancia a fragmentación.

La aprobación final de plataforma corresponde a `@JonatanGarbuyo`.