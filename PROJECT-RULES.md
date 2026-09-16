# Reglas operativas del proyecto

Este repositorio es la base de conocimiento compartida del proyecto Camila Online. Debe permitir continuar el trabajo desde otro chat o por otro usuario sin depender del historial de conversación anterior.

## 1. Fuente de verdad

- Las decisiones, investigaciones, dudas abiertas y contexto relevante deben quedar en este repositorio.
- Los chats son temporales; el repositorio es persistente.
- Antes de continuar trabajo en un chat nuevo, leer como mínimo:
  - `README.md`
  - `PROJECT-RULES.md`
  - `CONTEXT.md`
  - `docs/wayfinder/map.md`
  - los issues abiertos de Wayfinder relevantes.
- No asumir que una conversación anterior seguirá disponible.

## 2. Privacidad y secretos

No guardar en este repositorio:

- contraseñas;
- tokens o API keys;
- datos de tarjetas;
- secretos de aplicaciones;
- credenciales de pagos, Meta, WhatsApp, Tiendanube, correo o cualquier proveedor;
- documentos personales;
- datos privados de clientes que no sean necesarios para una decisión;
- información sensible que no deba quedar en GitHub.

Cuando una integración requiera una credencial, documentar únicamente **qué credencial hace falta y dónde debe configurarse**, nunca su valor.

Si un usuario comparte accidentalmente un secreto, advertir inmediatamente que no debe publicarse ni persistirse en el repo y recomendar revocarlo o rotarlo cuando corresponda.

## 3. Usuarios no técnicos y seguridad

Cuando una acción pueda generar un problema relevante —por ejemplo exposición de datos, cobros, pérdida de información, cambios irreversibles, acceso público o configuración insegura— advertir antes de ejecutarla.

Las advertencias dirigidas a personas no técnicas deben:

- usar lenguaje simple;
- explicar qué podría pasar;
- evitar jerga innecesaria;
- indicar la opción segura recomendada;
- diferenciar claramente entre un riesgo real y una precaución menor.

## 4. Autoridad para decisiones finales

**JonatanGarbuyo es el owner de las decisiones finales del proyecto.**

- Cualquier usuario puede investigar, proponer alternativas, documentar hallazgos y discutir trade-offs.
- Una recomendación no es una decisión final hasta que JonatanGarbuyo la apruebe explícitamente.
- Ningún otro usuario debe cerrar un ticket de decisión como resuelto en nombre de Jonatan.
- Si una decisión está madura pero pendiente de aprobación, debe quedar marcada como `needs-owner-approval`.
- Cuando haya una decisión lista para aprobar:
  1. resumir alternativas y trade-offs en el issue;
  2. indicar la recomendación propuesta;
  3. asignar el issue a `JonatanGarbuyo`;
  4. mencionar `@JonatanGarbuyo` en un comentario;
  5. esperar su aprobación antes de incorporarla como decisión final.

## 5. Roles

### JonatanGarbuyo

- owner de decisiones finales;
- único rol de desarrollo del proyecto;
- puede ejecutar código, desarrollar integraciones o implementar software cuando el proyecto llegue a esa etapa.

### Otros usuarios del proyecto

- discovery;
- investigación;
- relevamiento del negocio;
- comparación de servicios;
- documentación;
- discusión de alternativas;
- validación funcional y operativa.

No deben asumir tareas de desarrollo ni ejecución de código. Si aparece una necesidad técnica que requiere desarrollo, documentarla como decisión o requerimiento y dejarla para JonatanGarbuyo.

## 6. Chat como soporte operativo oficial

Para Camila y otros operadores no técnicos, el chat de este Project es el **canal oficial de ayuda operativa del proyecto**.

Cuando recibas una duda de operación:

1. priorizar la información de `/wiki/`;
2. usar el resto del repo como contexto interno cuando haga falta;
3. explicar los pasos en lenguaje simple y accionable;
4. indicar cómo verificar que el resultado quedó bien;
5. si la duda depende de una función vigente de un proveedor, verificar documentación actual antes de dar instrucciones cuando sea material;
6. no pedir secretos, contraseñas, códigos de verificación, tokens ni datos sensibles;
7. si la solución es reusable, persistirla luego en `/wiki/` en vez de dejarla solo en el chat.

No exponer Wayfinder, research interno o discusiones técnicas a un operador salvo que sea necesario para responder su problema.

El chat del proyecto no sustituye al soporte del proveedor cuando el incidente requiere acciones que solo ese proveedor puede ejecutar, por ejemplo bloqueos de cuenta, verificación de identidad, fondos retenidos, caídas del servicio o incidencias logísticas que dependen del transportista. En esos casos, ayudar a diagnosticar, preparar la consulta y entender la respuesta.

Guía para operadores: `wiki/ayuda-chat.md`.

## 7. Inicio obligatorio de un chat nuevo

Si otro usuario empieza un nuevo chat para trabajar en este proyecto, el asistente debe primero:

1. cargar este repositorio como contexto;
2. leer las reglas y el mapa Wayfinder;
3. inspeccionar los issues relevantes;
4. cargar desde `mattpocock/skills` las skills necesarias para la tarea.

Si el usuario es Camila u otro operador y llega con una duda concreta de administración, después del bootstrap debe priorizar `/wiki/` y ayudar con el problema actual antes de introducir trabajo de discovery no relacionado.

Para discovery y decisiones grandes, usar como base:

- `wayfinder`;
- `grilling`;
- `domain-modeling`;
- `research` cuando se necesiten hechos externos;
- `prototype` solo si hace falta un artefacto barato para responder una pregunta concreta.

No asumir que las skills ya están cargadas porque lo estuvieron en otro chat.

## 8. Wayfinder

El proyecto usa Wayfinder para trabajo de discovery prolongado.

- El mapa principal vive en GitHub Issues y se refleja en `docs/wayfinder/map.md`.
- Los tickets representan preguntas o decisiones, no tareas de implementación.
- Una investigación puede concluir con una propuesta, pero una decisión final requiere aprobación del owner.
- Mantener el mapa actualizado para que un chat nuevo pueda identificar la frontera sin leer conversaciones antiguas.

## 9. Documentación durable

Guardar únicamente información útil para retomar el proyecto:

- decisiones aprobadas y su motivo;
- alternativas evaluadas;
- hechos verificados y fecha de verificación;
- restricciones del negocio;
- problemas abiertos;
- riesgos relevantes;
- enlaces a fuentes primarias;
- próximos puntos de decisión;
- procedimientos operativos y soluciones repetibles en `/wiki/`.

Evitar transcripciones completas de conversaciones y ruido temporal.
