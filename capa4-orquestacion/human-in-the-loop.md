# Human-in-the-Loop

> **En una oración:** Es el punto del proceso donde una persona debe revisar y aprobar antes de que la IA continúe con el siguiente paso.

---

## ¿Qué es?
Human-in-the-loop (HITL) es el principio de diseño que mantiene al humano como punto de control en momentos críticos de un flujo automatizado. No es "la IA hace todo y el humano revisa al final" — es "la IA trabaja, pero pausa en puntos específicos para que una persona decida si seguir".

Los momentos más comunes para incluir HITL:
- Antes de ejecutar una acción irreversible (enviar un email, borrar datos, hacer una compra).
- Cuando la confianza del sistema es baja o la tarea es ambigua.
- En decisiones que tienen consecuencias legales, éticas o financieras.
- Cuando el resultado será publicado o enviado a clientes.

La pregunta de diseño clave es: **¿qué puede salir muy mal si la IA se equivoca aquí?** Si la respuesta es "bastante", ahí necesitas HITL.

---

## Analogía
Es como el **piloto automático de un avión**. El avión puede navegar solo durante horas, pero antes de maniobras complejas como el aterrizaje, el sistema alerta a los pilotos humanos para que tomen el control. La automatización hace el trabajo pesado; el humano conserva la decisión crítica.

---

## 🧪 Pruébalo
Diseña mentalmente (o en papel) un proceso de atención al cliente automatizado con IA:

1. IA recibe el mensaje del cliente.
2. IA clasifica el problema (urgente / normal / spam).
3. **HITL:** Si es "urgente", ¿la IA responde sola o un humano revisa primero?
4. IA redacta la respuesta.
5. **HITL:** ¿La IA envía directamente o el agente humano aprueba antes de enviar?

**¿Qué observar?** Cada vez que pones un "checkpoint" humano, agregas latencia pero reduces el riesgo de un error costoso. El arte del diseño de sistemas con IA es encontrar el balance correcto: demasiado HITL lo hace lento; muy poco lo hace impredecible.

---

## 📎 Para profundizar
- 📝 [Anthropic — Human-in-the-loop patterns](https://docs.anthropic.com/en/docs/build-with-claude/human-in-the-loop) — cuándo y cómo implementarlo en sistemas reales.
- 📝 [AI Snake Oil — "Automation vs. Augmentation"](https://www.aisnakeoil.com) — perspectiva crítica sobre cuándo la IA no debería decidir sola.
- 🎥 [LangChain — Breakpoints and human approval](https://www.youtube.com/watch?v=9BPCV5TYPmg) — implementación práctica con código (nivel intermedio).
