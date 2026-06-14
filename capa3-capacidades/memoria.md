# Memoria en IA

> **En una oración:** La capacidad de un sistema de IA de retener y usar información de interacciones pasadas para mejorar respuestas futuras.

---

## ¿Qué es?
La "memoria" en IA no es una sola cosa — hay al menos cuatro tipos distintos, y confundirlos lleva a expectativas incorrectas:

| Tipo | Qué es | Ejemplo |
|------|--------|---------|
| **Contexto (in-context)** | Todo lo que está en la conversación actual | El chat que tienes abierto ahora |
| **Externa (external)** | Base de datos fuera del modelo que se consulta | La "memoria" de ChatGPT que guarda preferencias |
| **Episódica** | Resúmenes de sesiones pasadas inyectados en nuevas sesiones | "En tu última sesión hablamos de X..." |
| **Del modelo (paramétrica)** | Lo que aprendió durante el entrenamiento | Todo lo que "sabe" el modelo base |

Cuando ves que ChatGPT "te recuerda", es memoria externa: una base de datos normal guardó un resumen de conversaciones anteriores, y ese resumen se inyecta en el prompt de la nueva sesión. El modelo en sí sigue sin recordar nada.

---

## Analogía
Imagina cuatro sistemas de memoria humana:
- **Contexto** = Lo que tienes en mente ahora mismo en esta conversación.
- **Memoria externa** = Tu agenda y cuaderno de notas.
- **Episódica** = El resumen que alguien te hizo de lo que pasó ayer.
- **Paramétrica** = Todo lo que aprendiste en la escuela y ya no necesitas consultar.

El LLM solo tiene la última de manera nativa. Las demás se construyen encima con herramientas adicionales.

---

## 🧪 Pruébalo
**Para ver la memoria externa en acción:**
1. En ChatGPT, ve a Configuración → Personalización → Memoria.
2. Observa qué tiene guardado sobre ti.
3. Borra un elemento y verifica que deja de mencionarlo.

**Para ver la ausencia de memoria nativa:**
1. Cuéntale algo personal en una conversación.
2. Cierra esa ventana y abre una *nueva* conversación.
3. Pregunta si recuerda lo que te contó antes.

**¿Qué observar?** En el segundo experimento, no tiene idea. La memoria "vive" en los sistemas externos, no en el modelo. Desactivar la función de memoria en ChatGPT lo convierte en un modelo completamente amnésico de sesión a sesión.

---

## 📎 Para profundizar
- 📝 [Lilian Weng — "LLM Powered Autonomous Agents"](https://lilianweng.github.io/posts/2023-06-23-agent/) — el artículo de referencia sobre memoria en sistemas agénticos (nivel técnico pero muy completo).
- 📝 [Simon Willison — Memory in AI systems](https://simonwillison.net/tags/memory/) — observaciones prácticas sin jerga innecesaria.
- 🎥 [AI Explained — How ChatGPT memory works](https://www.youtube.com/watch?v=v2IzULvlXQ8) — desmontando el mito de la "memoria real" con evidencia.
