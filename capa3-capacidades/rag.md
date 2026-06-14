# RAG (Retrieval-Augmented Generation)

> **En una oración:** Es hacer que la IA busque información en tus propios documentos antes de responder, en lugar de depender solo de su entrenamiento.

---

## ¿Qué es?
RAG combina dos sistemas: un buscador y un generador.

1. **Retrieval (recuperación):** Cuando haces una pregunta, el sistema busca en tu base de documentos (PDFs, notas, base de datos, etc.) los fragmentos más relevantes.
2. **Augmented Generation (generación aumentada):** Esos fragmentos se agregan al contexto del LLM como si fueran parte del prompt. El modelo genera su respuesta basándose en *tu información real*, no en lo que aprendió hace meses.

**Por qué importa:** Sin RAG, si le preguntas a la IA sobre tu empresa, tus políticas internas o un documento específico, inventa. Con RAG, trabaja con la fuente real.

---

## Analogía
Es como darle a un investigador muy inteligente (el LLM) acceso a **tu biblioteca personal** antes de responderte. Sin acceso, improvisa con lo que recuerda. Con acceso, primero busca en tus archivos, encuentra los párrafos relevantes, y *luego* responde basándose en lo que encontró.

---

## 🧪 Pruébalo
**Sin código:** Usa [NotebookLM de Google](https://notebooklm.google.com) (gratuito):
1. Sube un PDF o documento propio.
2. Hazle preguntas sobre el contenido.
3. Observa cómo cita partes específicas del documento en sus respuestas.

**¿Qué observar?** NotebookLM no inventa: ancla cada respuesta a citas del documento. Eso es RAG en acción, sin que tengas que escribir una sola línea de código.

---

## 📎 Para profundizar
- 🔧 [NotebookLM](https://notebooklm.google.com) — la forma más rápida de experimentar RAG sin código.
- 📝 [Anthropic — RAG overview](https://docs.anthropic.com/en/docs/build-with-claude/retrieval-augmented-generation) — qué es y cuándo usarlo vs. fine-tuning.
- 🎥 [LangChain — RAG from scratch](https://www.youtube.com/watch?v=sVcwVQRHIc8) — si quieres construirlo tú mismo (Python, nivel intermedio).
