# Workflow

> **En una oración:** Es una secuencia predefinida de pasos que una IA ejecuta en orden para completar una tarea compleja.

---

## ¿Qué es?
Un workflow es un flujo de trabajo donde cada paso tiene un input, una acción y un output que alimenta al siguiente paso. A diferencia de un agente (que decide autónomamente qué hacer), un workflow sigue una ruta definida por el humano o el sistema que lo diseñó.

Piensa en ello como una receta: los pasos están fijos. El valor está en la automatización y consistencia, no en la autonomía.

**Cuándo usar un workflow vs. un agente:**
- **Workflow:** Cuando el proceso es repetible y bien conocido. Procesar facturas, generar reportes, responder FAQs.
- **Agente:** Cuando la tarea es abierta y requiere decisiones en tiempo real. Investigar un mercado desconocido, resolver un bug nuevo.

---

## Analogía
Es como una **línea de ensamblaje en una fábrica**. Cada estación hace exactamente lo que le corresponde, en el orden correcto, sin improvisar. La eficiencia está garantizada; la flexibilidad, no.

---

## 🧪 Pruébalo
Crea un mini-workflow manual en cualquier IA:

1. **Paso 1:** "Toma este email de un cliente enojado y extrae: 1) el problema principal, 2) el tono emocional, 3) lo que pide explícitamente." [Pega un email real o inventado]
2. **Paso 2:** "Basándote en los 3 puntos que extrajiste, redacta una respuesta empática de no más de 100 palabras."
3. **Paso 3:** "Revisa la respuesta anterior y evalúa si cumple: ¿reconoce el problema? ¿ofrece solución? ¿tono adecuado? Califica del 1 al 10."

**¿Qué observar?** Cada paso usa el output del anterior como input. Eso es un workflow: input → proceso → output → input del siguiente. En sistemas reales, esto se automatiza con herramientas como n8n, Zapier o LangChain.

---

## 📎 Para profundizar
- 🔧 [n8n](https://n8n.io) — herramienta visual gratuita para crear workflows con IA sin código.
- 🔧 [LangChain — Chains](https://python.langchain.com/docs/modules/chains/) — implementación técnica de workflows en Python.
- 📝 [Anthropic — Workflow patterns](https://docs.anthropic.com/en/docs/build-with-claude/workflow) — cuándo usar workflows vs. agentes, con criterios claros.
