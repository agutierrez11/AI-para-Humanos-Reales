# Tools / Skills (Herramientas)

> **En una oración:** Son las "manos" que le das a la IA para que pueda hacer cosas en el mundo real, no solo generar texto.

---

## ¿Qué es?
Un LLM base solo puede generar texto. Las herramientas (tools) son funciones externas que el modelo puede invocar cuando decide que las necesita para completar una tarea:

- **Búsqueda web:** buscar información actualizada en internet.
- **Calculadora / intérprete de código:** ejecutar cálculos o código Python.
- **Acceso a archivos:** leer o escribir documentos.
- **APIs externas:** consultar el clima, reservar un vuelo, actualizar una hoja de cálculo.
- **Bases de datos:** buscar en tus propios datos estructurados.

El modelo no ejecuta las herramientas directamente — genera un "llamado" que el sistema externo ejecuta, y luego recibe el resultado para continuar respondiendo.

---

## Analogía
Es la diferencia entre un **consultor que solo da consejos verbales** y uno que también puede **abrir tu laptop, buscar en tus reportes y calcular proyecciones en Excel**. El conocimiento base es el mismo; las herramientas determinan qué puede hacer con él.

---

## 🧪 Pruébalo
1. Pregunta a ChatGPT (con búsqueda activada) o Gemini: **"¿Cuánto cuesta el dólar en México hoy?"**
2. Observa si aparece un ícono de búsqueda o cita una fuente con fecha de hoy.
3. Luego desactiva la búsqueda (si puedes) y haz la misma pregunta.

**¿Qué observar?** Con la herramienta de búsqueda activa, obtienes un dato real y actualizado. Sin ella, el modelo responde con el valor que tenía al momento de su entrenamiento, que puede tener meses o años de antigüedad — aunque responda con igual confianza.

---

## 📎 Para profundizar
- 📝 [OpenAI — Function calling](https://platform.openai.com/docs/guides/function-calling) — cómo se define una herramienta técnicamente.
- 📝 [Anthropic — Tool use](https://docs.anthropic.com/en/docs/build-with-claude/tool-use) — guía completa con ejemplos de código.
- 🎥 [AI Jason — Tool use in practice](https://www.youtube.com/watch?v=A5jGD6LWMJE) — video práctico mostrando herramientas reales funcionando.
