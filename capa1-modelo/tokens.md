# Tokens

> **En una oración:** Es la unidad mínima de texto con la que un LLM lee, procesa y genera lenguaje.

---

## ¿Qué es?
Un token no es exactamente una palabra ni un carácter: es un fragmento de texto que puede ser una palabra completa, parte de una palabra, o un signo de puntuación. Por ejemplo, la palabra "tokenización" se divide en varios tokens: `token`, `iza`, `ción`.

Los modelos no leen oraciones; leen secuencias de tokens. Esto tiene consecuencias prácticas: el costo de usar una API se mide en tokens consumidos, y el límite de lo que un modelo puede "leer de una vez" (su ventana de contexto) también se mide en tokens.

**Regla práctica:** 1 token ≈ 0.75 palabras en inglés. En español suele ser menos eficiente — el mismo texto ocupa más tokens.

---

## Analogía
Es como las **sílabas con las que aprendes a leer**. Tú lees "ma-te-má-ti-cas", no la palabra entera de un golpe. El LLM hace lo mismo, pero a una velocidad y escala incomprensible para un humano.

---

## 🧪 Pruébalo
1. Ve a [platform.openai.com/tokenizer](https://platform.openai.com/tokenizer).
2. Escribe el mismo párrafo en inglés y en español.
3. Observa cuántos tokens ocupa cada versión.

**¿Qué observar?** El texto en español generalmente ocupa más tokens que su equivalente en inglés. Esto explica por qué los modelos pueden parecer "menos capaces" en otros idiomas — no es el idioma, es la eficiencia con la que el modelo fue entrenado para tokenizarlo.

---

## 📎 Para profundizar
- 🎥 [Andrej Karpathy — "Let's build the GPT Tokenizer"](https://www.youtube.com/watch?v=zduSFxRajkE) — 2h pero te cambia cómo ves la IA.
- 🔧 [OpenAI Tokenizer (interactivo)](https://platform.openai.com/tokenizer) — ve en tiempo real cómo se corta tu texto.
- 📝 [Hugging Face — What are Tokens?](https://huggingface.co/learn/nlp-course/chapter2/4) — explicación técnica sin ser intimidante.
