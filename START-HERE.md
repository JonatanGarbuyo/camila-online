# START HERE — Camila Online

Este archivo es el punto de entrada canónico para cualquier chat nuevo que trabaje sobre este proyecto.

## Fuente de verdad

El repositorio `JonatanGarbuyo/camila-online` es la **fuente de verdad y base de conocimiento durable** del proyecto.

Los chats sirven para investigar, discutir y trabajar. Todo conocimiento que deba sobrevivir al chat —hallazgos, restricciones, decisiones propuestas, decisiones aprobadas, riesgos y próximos puntos de decisión— debe quedar documentado en el repositorio.

No asumir que otro chat conoce una conversación anterior si ese conocimiento no quedó persistido acá.

## Bootstrap obligatorio de cada chat

Antes de avanzar:

1. Leer `README.md`.
2. Leer `PROJECT-RULES.md`.
3. Leer `CONTEXT.md`.
4. Leer `docs/wayfinder/map.md`.
5. Revisar los Issues Wayfinder abiertos relevantes y sus comentarios.
6. Cargar desde `mattpocock/skills` las skills que correspondan a la tarea. Para discovery grande, usar `wayfinder` y sus dependencias relevantes (`grilling`, `domain-modeling`, `research`, `prototype` según corresponda).
7. Reconstruir el estado actual desde el repo antes de proponer trabajo nuevo.

## Al terminar trabajo significativo

Persistir en el repo solamente conocimiento durable, por ejemplo:

- investigación verificada y sus fuentes;
- restricciones descubiertas;
- decisiones propuestas y alternativas;
- decisiones aprobadas;
- riesgos o problemas detectados;
- cambios en el mapa Wayfinder;
- nuevas preguntas que deban resolverse después.

No guardar conversación transitoria, ruido ni duplicar información sin necesidad.

## Autoridad y decisiones

- Las decisiones finales requieren aprobación explícita de `@JonatanGarbuyo`.
- Otros usuarios pueden investigar, debatir, proponer y documentar alternativas.
- Una recomendación no es una decisión aprobada.
- Cuando una decisión esté madura para aprobación, dejarla claramente marcada, asignar/mencionar a `@JonatanGarbuyo` y no cerrarla como final hasta su confirmación.

## Desarrollo

- `@JonatanGarbuyo` es quien realiza desarrollo y ejecución de código.
- Los demás participantes del proyecto no deben ejecutar código ni hacer desarrollo productivo.
- Si aparece una necesidad técnica, documentarla como problema, requisito o decisión pendiente para que Jonatan la evalúe.
- El MVP actual prioriza soluciones no-code.

## Seguridad y privacidad

Nunca guardar en el repo:

- contraseñas;
- tokens;
- API keys;
- secretos;
- credenciales;
- datos privados de clientes;
- información sensible que no sea necesaria para el proyecto.

Si una persona no técnica está por realizar una acción riesgosa, insegura, costosa o difícil de revertir, alertarla antes en lenguaje simple: qué puede salir mal, qué impacto tendría y cuál es la alternativa más segura.

## Regla de continuidad

El objetivo es que cualquier integrante pueda abrir un chat nuevo dentro del Project de ChatGPT, leer este repositorio y continuar el trabajo sin necesitar el historial completo de chats anteriores.
