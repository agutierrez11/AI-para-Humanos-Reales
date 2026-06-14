# Contexto (Context Window)

> **En una oración:** Es la cantidad de texto que un modelo puede leer y recordar dentro de una misma conversación.

---

## ¿Qué es?
La ventana de contexto es el límite de "memoria de trabajo" de un LLM durante una conversación. Todo lo que entra — tus mensajes, las respuestas del modelo, documentos que adjuntas — ocupa espacio en esa ventana.

Cuando la conversación supera ese límite, el modelo empieza a "olvidar" lo que dijo al principio. No hay aviso. Simplemente deja de tener acceso a esa parte del historial.

Los modelos modernos tienen ventanas enormes (GPT-4o: ~128k tokens; Gemini 1.5 Pro: hasta 1 millón de tokens), pero el problema de qué incluir y cómo organizarlo sigue siendo relevante para la calidad de las respuestas.

---

## Analogía
Imagina que tu memoria de trabajo es una **mesa de trabajo**. Puedes tener muchos papeles sobre la mesa, pero cuando se llena, tienes que empujar algunos al piso para poner nuevos. Lo que cae al piso ya no puedes verlo aunque sigue existiendo en algún cajón.

---

## 🧪 Pruébalo
1. Empieza una conversación larga con cualquier IA — copia y pega un texto muy largo (un artículo completo).
2. Después de muchos mensajes, pregúntale algo sobre el inicio de la conversación.
3. Observa si la respuesta es coherente o empieza a divagar.

**¿Qué observar?** En conversaciones muy largas, el modelo puede contradecir algo que dijo al principio o "no recordar" instrucciones que diste hace muchos mensajes. Eso es el límite del contexto en acción.

---

## 📎 Para profundizar
- 📝 [Anthropic — Long context tips](https://docs.anthropic.com/en/docs/build-with-claude/long-context-tips) — consejos prácticos de los creadores de Claude.
- 🎥 [Andrej Karpathy — "Intro to Large Language Models"](https://www.youtube.com/watch?v=zjkBMFhNj_g) — explica el contexto desde los fundamentos (1h que vale la pena).
- 🔧 [LLM Context Length Tracker](https://github.com/rahulnyk/knowledge_graph) — comparativa actualizada de ventanas de contexto por modelo.
