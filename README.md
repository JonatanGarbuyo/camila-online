# Camila Online

Repositorio de discovery, decisiones y documentación para habilitar una tienda online de alcance nacional para el negocio de Camila.

Este repositorio funciona como **base de conocimiento persistente del proyecto**: los chats son temporales; las decisiones, investigaciones, dudas abiertas y contexto que deban sobrevivir entre conversaciones deben quedar documentados acá.

## Continue from here

Para retomar el proyecto desde un chat nuevo, compartir este repositorio:

**https://github.com/JonatanGarbuyo/camila-online**

Mensaje recomendado para iniciar el chat:

```text
Continuá el proyecto Camila Online desde este repositorio:
https://github.com/JonatanGarbuyo/camila-online

Antes de avanzar:
1. Leé README.md, PROJECT-RULES.md, docs/CHAT-BOOTSTRAP.md y CONTEXT.md.
2. Revisá el mapa Wayfinder y los GitHub Issues abiertos.
3. Cargá desde https://github.com/mattpocock/skills las skills de Matt que correspondan; para discovery prolongado, empezá por wayfinder y sus dependencias.
4. Tratá el repositorio como fuente de verdad y memoria persistente del proyecto.
5. No guardes secretos ni datos sensibles.
6. Si el usuario no es técnico, explicá riesgos o acciones inseguras en lenguaje simple y proponé una alternativa segura.
7. No ejecutes código ni hagas desarrollo salvo que @JonatanGarbuyo lo pida explícitamente.
8. Ninguna decisión final queda aprobada sin confirmación explícita de @JonatanGarbuyo.

Primero reconstruí el estado desde el repo y resumí: decisiones cerradas, decisiones pendientes y frontera actual de Wayfinder. No empieces una nueva línea de trabajo antes de hacerlo.
```

### Link directo a ChatGPT

Si se usa un enlace compartido de un Project de ChatGPT, el destinatario puede entrar al proyecto y abrir un chat nuevo desde allí. El repositorio sigue siendo la fuente de verdad durable.

ChatGPT no documenta actualmente un parámetro URL estable que cree un chat nuevo y envíe automáticamente el primer mensaje. En algunas superficies `?prompt=<texto>` puede precargar el compositor, pero debe tratarse como una comodidad no garantizada, no como parte del protocolo del proyecto.

Si se usa ese mecanismo, el texto mínimo a precargar debe ser:

```text
Continuá desde https://github.com/JonatanGarbuyo/camila-online y seguí la sección "Continue from here" del README.
```

## Objetivo

Diseñar un MVP de e-commerce **no-code**, de bajo o nulo costo fijo, que cubra:

- catálogo online;
- links desde Facebook e Instagram;
- pago online;
- envíos nacionales y cobertura/seguro;
- atención por WhatsApp;
- medición de adquisición, referidos y ventas.

## Principio de trabajo

Primero resolvemos decisiones e investigamos restricciones con Wayfinder. No se desarrolla software propio mientras una solución administrada/no-code cubra razonablemente el problema.

**Las decisiones finales requieren aprobación explícita de `@JonatanGarbuyo`.** Otros participantes pueden investigar, debatir y proponer, pero no cerrar decisiones finales en su nombre.

## Al iniciar un chat nuevo

Leer primero:

1. [Reglas del proyecto](PROJECT-RULES.md)
2. [Bootstrap para chats](docs/CHAT-BOOTSTRAP.md)
3. [Contexto y vocabulario](CONTEXT.md)
4. [Mapa Wayfinder](docs/wayfinder/map.md)
5. Issues Wayfinder abiertos relevantes

Luego cargar desde `mattpocock/skills` las skills que correspondan. Para discovery prolongado: `wayfinder`, `grilling`, `domain-modeling` y, según la pregunta, `research` o `prototype`.

## Seguridad

No guardar secretos, contraseñas, tokens, API keys ni datos privados de clientes en este repositorio. Las alertas para usuarios no técnicos deben explicar los riesgos en lenguaje simple y proponer una alternativa segura.

## Estado

El proyecto está en fase de **discovery / Wayfinder**.

- [Reglas operativas](PROJECT-RULES.md)
- [Bootstrap para chats](docs/CHAT-BOOTSTRAP.md)
- [Mapa Wayfinder](docs/wayfinder/map.md)
- [Opciones iniciales](docs/research/options.md)
- [Pagos](docs/research/payments.md)
- [Envíos y seguros](docs/research/shipping-insurance.md)
- [Métricas y atribución](docs/research/measurement.md)
- [Contexto y vocabulario](CONTEXT.md)
