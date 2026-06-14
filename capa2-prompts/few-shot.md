# Few-Shot Prompting

> **En una oración:** Es mostrarle a la IA ejemplos concretos de lo que quieres para que entienda el patrón sin explicaciones largas.

---

## ¿Qué es?
En lugar de explicar con palabras qué tipo de respuesta esperas, le muestras 2-5 ejemplos del formato entrada → salida que quieres. El modelo infiere el patrón y lo aplica a tu caso real.

- **Zero-shot:** Sin ejemplos ("Clasifica este texto como positivo o negativo").
- **One-shot:** Un ejemplo antes de tu pregunta real.
- **Few-shot:** 2 a 5 ejemplos. El punto óptimo para la mayoría de tareas.

Es especialmente poderoso cuando quieres un formato muy específico de respuesta, un tono particular o una lógica de clasificación que sería difícil de describir con palabras.

---

## Analogía
Es como **enseñarle a alguien un trabajo mostrándole tres ejemplos reales** en lugar de darle un manual de instrucciones. Después de ver tres facturas bien redactadas, entiende el formato mejor que leyendo una descripción de cómo debe verse una factura.

---

## 🧪 Pruébalo
Pega esto en cualquier IA:

```
Clasifica el sentimiento de estas reseñas:

Reseña: "El producto llegó roto y el servicio fue pésimo." → Negativo
Reseña: "Funciona exactamente como esperaba, sin más." → Neutral
Reseña: "¡Increíble! Superó todas mis expectativas." → Positivo

Ahora clasifica esta:
Reseña: "Tardó más de lo prometido pero al final llegó en buen estado."
```

**¿Qué observar?** Sin los ejemplos, la IA podría clasificarlo como positivo, negativo o neutro dependiendo del modelo. Con los ejemplos, el patrón está claro y la respuesta debería ser "Neutral" de forma consistente. Los ejemplos anclan el comportamiento mucho más que las instrucciones.

---

## 📎 Para profundizar
- 📝 [Anthropic — Few-shot prompting](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/use-examples) — con ejemplos reales de cuándo usarlo.
- 📝 [Prompt Engineering Guide — Few-Shot](https://www.promptingguide.ai/techniques/fewshot) — comparativa técnica con investigación detrás.
- 🎥 [Andrew Ng — Prompting Best Practices](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/) — curso gratuito de 1h con Jupyter Notebooks ejecutables.
