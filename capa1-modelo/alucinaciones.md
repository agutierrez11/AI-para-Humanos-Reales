# Alucinaciones (Hallucinations)

> **En una oración:** Cuando la IA genera información falsa con total confianza, como si fuera un hecho verificado.

---

## ¿Qué es?
Una alucinación es cuando un LLM produce texto que suena perfectamente razonable, coherente y seguro de sí mismo... pero que es incorrecto, inventado o directamente inexistente.

No es que la IA "mienta" con intención — simplemente su objetivo es generar texto plausible, no necesariamente verdadero. Si no tiene información suficiente sobre algo, llena los espacios en blanco con patrones que suenan correctos.

Los casos más comunes:
- **Citas inventadas:** "Según el estudio de González et al. (2021)..." — el estudio no existe.
- **Datos numéricos falsos:** estadísticas que suenan precisas pero son fabricadas.
- **Hechos históricos alterados:** fechas, nombres o eventos ligeramente incorrectos.
- **Código que no funciona:** funciones o APIs que no existen en la realidad.

---

## Analogía
Es como un **estudiante que no estudió para el examen pero tiene gran habilidad para sonar convincente**. Escribe respuestas largas, con vocabulario técnico, bien estructuradas. Son plausibles en su forma, pero el contenido puede ser pura invención.

---

## 🧪 Pruébalo
Pregúntale a cualquier IA:
> "¿Puedes citar tres papers académicos publicados entre 2020 y 2023 sobre el impacto de los LLMs en la educación secundaria en Latinoamérica?"

Luego busca en Google Scholar si esos papers existen de verdad.

**¿Qué observar?** Es muy probable que al menos uno de los papers citados (autores, título, revista, año) sea completamente inventado. El modelo no sabe que no sabe — genera lo que "debería" existir.

---

## 📎 Para profundizar
- 📝 [Simon Willison — "Hallucinations"](https://simonwillison.net/2023/Dec/31/ai-in-2023/) — observaciones prácticas del uno de los mejores observadores de IA sin hype.
- 📝 [Anthropic — Why AI systems hallucinate](https://www.anthropic.com/research) — perspectiva técnica de los creadores de Claude.
- 🎥 [3Blue1Brown — "Attention in transformers"](https://www.youtube.com/watch?v=eMlx5fFNoYc) — para entender *por qué* ocurren a nivel técnico (no es requisito, pero es fascinante).

> ⚠️ **Regla práctica:** Si la IA te da un dato específico (número, nombre, fecha, cita), verifica siempre en una fuente independiente antes de usarlo.
