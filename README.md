# Camila Online

Repositorio de discovery, decisiones, investigación y documentación operativa para habilitar y administrar tiendas online.

Este repositorio funciona como **base de conocimiento persistente del proyecto**: los chats son temporales; las decisiones, investigaciones, dudas abiertas, playbooks y contexto que deban sobrevivir entre conversaciones deben quedar documentados acá.

## Continue from here

Para cualquier chat nuevo, empezar por [`START-HERE.md`](START-HERE.md).

Repositorio: **https://github.com/JonatanGarbuyo/camila-online**

Mensaje mínimo sugerido:

```text
Continuá desde https://github.com/JonatanGarbuyo/camila-online y seguí START-HERE.md antes de avanzar.
```

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

## Fuente de verdad y conocimiento

Usamos GitHub para tres tipos de conocimiento durable:

1. **Issues:** preguntas, investigación, discusión, decisiones y aprobaciones.
2. **`docs/research/`:** hechos verificados, comparaciones y fuentes externas.
3. **`docs/playbook/`:** manual operativo para levantar, lanzar y administrar tiendas.

No hace falta otra base de conocimiento por ahora. Si más adelante Camila necesita una interfaz de manual más visual, se puede publicar/replicar el playbook en otra herramienta, pero GitHub debe seguir siendo la fuente canónica para evitar versiones contradictorias.

## Estado de plataforma

**La plataforma final todavía no está decidida.**

- Tiendanube Inicial es la baseline a validar por su costo fijo $0 y su encaje local en Argentina.
- Empretienda es el fallback pago de bajo costo.
- Odoo One App Free quedó registrado como alternativa gratuita secundaria con mayor complejidad.
- La decisión final vive en el issue #9 y requiere aprobación explícita de `@JonatanGarbuyo`.

Ver:

- [Mapa Wayfinder](docs/wayfinder/map.md)
- [Comparación de plataformas, precios y SEO](docs/research/platforms-pricing-seo.md)
- [Skeleton del playbook operativo](docs/playbook/README.md)

## Principio de trabajo

Primero resolvemos decisiones e investigamos restricciones con Wayfinder. No se desarrolla software propio mientras una solución administrada/no-code cubra razonablemente el problema.

**Las decisiones finales requieren aprobación explícita de `@JonatanGarbuyo`.** Otros participantes pueden investigar, debatir y proponer, pero no cerrar decisiones finales en su nombre.

## Al iniciar un chat nuevo

Leer primero:

1. [START-HERE](START-HERE.md)
2. [Reglas del proyecto](PROJECT-RULES.md)
3. [Bootstrap para chats](docs/CHAT-BOOTSTRAP.md)
4. [Contexto y vocabulario](CONTEXT.md)
5. [Mapa Wayfinder](docs/wayfinder/map.md)
6. Issues Wayfinder abiertos relevantes

Luego cargar desde `mattpocock/skills` las skills que correspondan.

## Seguridad

No guardar secretos, contraseñas, tokens, API keys ni datos privados de clientes en este repositorio. Las alertas para usuarios no técnicos deben explicar los riesgos en lenguaje simple y proponer una alternativa segura.
