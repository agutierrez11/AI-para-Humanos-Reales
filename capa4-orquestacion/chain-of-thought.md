# Chain of Thought (Cadena de Pensamiento)

> **En una oración:** Es pedirle a la IA que muestre su razonamiento paso a paso antes de dar una respuesta final.

---

## ¿Qué es?
Chain of Thought (CoT) es una técnica de prompting donde se le pide al modelo que "piense en voz alta" — que explique el proceso de razonamiento intermedio antes de llegar a una conclusión. Esto mejora drásticamente la precisión en tareas que requieren lógica, matemáticas o análisis en múltiples pasos.

Sin CoT, el modelo intenta saltar directamente a la respuesta y puede equivocarse en el camino. Con CoT, al articular cada paso intermedio, el modelo se autocontrola y detecta inconsistencias antes de llegar a la respuesta final.

**Truco simple que funciona:** Agregar "Piensa paso a paso" o "Razona en voz alta antes de responder" al final de tu prompt.

---

## Analogía
Es la diferencia entre un estudiante que anota el procedimiento completo del examen y uno que solo escribe el resultado final. El que muestra el proceso puede encontrar su error a mitad del camino y corregirlo; el que solo da el resultado, no.

---

## 🧪 Pruébalo
Resuelve el mismo problema con y sin CoT:

**Sin CoT:**
> "María tiene 3 veces más manzanas que Juan. Juan tiene 4 manzanas menos que Pedro. Pedro tiene 12 manzanas. ¿Cuántas manzanas tiene María?"

**Con CoT:**
> "María tiene 3 veces más manzanas que Juan. Juan tiene 4 manzanas menos que Pedro. Pedro tiene 12 manzanas. ¿Cuántas manzanas tiene María? **Piensa paso a paso.**"

**¿Qué observar?** La versión con CoT suele ser más precisa porque el modelo va calculando cada relación por separado. Sin CoT, puede confundir las relaciones y dar un número incorrecto con total confianza. Funciona especialmente bien en problemas matemáticos, lógica y análisis de textos complejos.

---

## 📎 Para profundizar
- 📝 [Paper original de Wei et al. (2022)](https://arxiv.org/abs/2201.11903) — "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models" — el paper que popularizó la técnica.
- 📝 [Prompt Engineering Guide — CoT](https://www.promptingguide.ai/techniques/cot) — resumen aplicado con ejemplos.
- 🎥 [Yannic Kilcher — Explaining CoT paper](https://www.youtube.com/watch?v=4hqFPzGXBGw) — análisis del paper original en video (nivel técnico accesible).
