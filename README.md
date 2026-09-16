# Camila Online

Repositorio de discovery, decisiones, investigación y documentación operativa para habilitar y administrar tiendas online.

Este repositorio funciona como **base de conocimiento persistente del proyecto**: los chats son temporales; las decisiones, investigaciones, dudas abiertas, playbooks y contexto que deban sobrevivir entre conversaciones deben quedar documentados acá.

## Dos entradas distintas

### Para Camila y otros operadores no técnicos

👉 [Guía práctica de la tienda](docs/INDEX.md)

Esa guía contiene solo procedimientos operativos claros en español: publicación de productos, catálogo, pagos, envíos, atención, métricas y operación diaria a medida que se vayan completando.

No debe incluir Wayfinder, Issues ni discusiones internas del proyecto.

### Para chats, agentes y trabajo de proyecto

👉 [START-HERE.md](START-HERE.md)

Desde ahí se reconstruyen reglas, contexto, Wayfinder, Issues e investigación vigente.

## Objetivo

Diseñar un MVP de e-commerce **no-code**, de bajo o nulo costo fijo, que cubra:

- catálogo online;
- links desde Facebook e Instagram;
- pago online;
- envíos nacionales y cobertura/seguro;
- atención por WhatsApp;
- SEO y buenas prácticas de publicación;
- medición de adquisición, referidos y ventas.

El primer caso es un comercio de ropa. El aprendizaje debe convertirse progresivamente en un **playbook reusable** para otros comercios, sin construir prematuramente una plataforma/SaaS propia.

## Organización del conocimiento

- **Issues:** preguntas, investigación en curso, discusión y decisiones.
- **`docs/research/`:** hechos verificados, comparaciones y fuentes externas.
- **`docs/wayfinder/`:** estado de discovery y planificación.
- **`docs/playbook/`:** manual operativo para personas no técnicas.
- **`docs/INDEX.md`:** portada simple de la guía operativa.

## Estado de plataforma

**La plataforma final todavía no está decidida.** La shortlist activa es:

1. Tiendanube
2. DonWeb SitioSimple
3. Empretienda

Las cuentas de prueba se crearán y operarán manualmente por Camila o Jonatan. La decisión final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.

## Principio de trabajo

Primero resolvemos decisiones e investigamos restricciones con Wayfinder. No se desarrolla software propio mientras una solución administrada/no-code cubra razonablemente el problema.

## Seguridad

No guardar secretos, contraseñas, tokens, API keys ni datos privados de clientes en este repositorio. Las alertas para usuarios no técnicos deben explicar los riesgos en lenguaje simple y proponer una alternativa segura.