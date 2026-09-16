# Camila Online

Repositorio de discovery, decisiones, investigación y documentación operativa para habilitar y administrar tiendas online.

Este repositorio funciona como **base de conocimiento persistente del proyecto**: los chats son temporales; las decisiones, investigaciones, dudas abiertas y procedimientos que deban sobrevivir entre conversaciones deben quedar documentados acá.

## Dos entradas distintas

### Para Camila y otros operadores no técnicos

👉 [Wiki práctica de la tienda](wiki/README.md)

`/wiki/` reemplaza, dentro de este repositorio, el uso de GitHub Wiki que no podemos mantener desde este entorno.

La wiki contiene solamente procedimientos claros en español: publicación de productos, catálogo, pagos, envíos, atención, métricas y operación diaria a medida que se vayan completando.

No debe incluir Wayfinder, Issues, comparaciones de plataformas ni discusiones internas del proyecto.

### Para chats, agentes y trabajo de proyecto

👉 [START-HERE.md](START-HERE.md)

Desde ahí se reconstruyen reglas, contexto, Wayfinder, Issues e investigación vigente.

## Objetivo

Diseñar un MVP de e-commerce **no-code**, de bajo o nulo costo fijo, que cubra catálogo online, links desde redes, pago online, envíos nacionales, atención por WhatsApp, SEO/publicación y medición.

El primer caso es un comercio de ropa. El aprendizaje debe convertirse progresivamente en una guía reusable para otros comercios, sin construir prematuramente una plataforma/SaaS propia.

## Organización del conocimiento

- **Issues:** preguntas, investigación en curso, discusión y decisiones.
- **`docs/research/`:** hechos verificados, comparaciones y fuentes externas.
- **`docs/wayfinder/`:** estado de discovery y planificación.
- **`wiki/`:** base de conocimiento práctica y procedimientos para operadores no técnicos.

## Estado de plataforma

**La plataforma final todavía no está decidida.** La shortlist activa quedó reducida a:

1. **Tiendanube**
2. **DonWeb SitioSimple**

**Empretienda fue descartada en esta etapa** frente a esas dos por menor documentación pública, dependencia de medios de pago externos y menor claridad operativa/accesos. Puede reabrirse solo si ambas finalistas fallan por una restricción concreta.

Las cuentas de prueba se crearán y operarán manualmente por Camila o Jonatan. La decisión final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.

## Principio de trabajo

Primero resolvemos decisiones e investigamos restricciones con Wayfinder. No se desarrolla software propio mientras una solución administrada/no-code cubra razonablemente el problema.

## Seguridad

No guardar secretos, contraseñas, tokens, API keys ni datos privados de clientes en este repositorio. Las alertas para usuarios no técnicos deben explicar los riesgos en lenguaje simple y proponer una alternativa segura.
