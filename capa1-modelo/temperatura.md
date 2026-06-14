# Temperatura (Temperature)

> **En una oración:** Es el parámetro que controla qué tan predecible o creativa es la respuesta de un modelo.

---

## ¿Qué es?
Cuando un modelo genera texto, en cada paso elige entre varias palabras posibles. La temperatura determina qué tan "atrevida" es esa elección:

- **Temperatura baja (0.0 – 0.3):** El modelo elige casi siempre la opción más probable. Las respuestas son consistentes, precisas y predecibles. Ideal para código, datos, respuestas factuales.
- **Temperatura alta (0.8 – 1.5):** El modelo considera opciones menos probables. Las respuestas son más variadas, creativas... y también más propensas a errores.

La mayoría de los chats públicos (ChatGPT, Claude) tienen temperatura moderada por defecto (~0.7). Puedes controlarlo directamente si usas las APIs.

---

## Analogía
Es como el **dial de un DJ entre "mezcla clásica probada" y "improvisación en vivo"**. En modo conservador suena igual cada vez. En modo creativo puede sorprenderte o hacer algo que no esperabas del todo.

---

## 🧪 Pruébalo
Pide esto tres veces seguidas sin cambiar nada:
> "Escribe el primer verso de un poema sobre el tiempo que pasa."

**¿Qué observar?** Probablemente recibas 3 respuestas distintas. Eso es la temperatura en acción: el modelo no es una función determinista, hay aleatoriedad controlada en cada respuesta.

Para comparar extremos, si tienes acceso a la API de OpenAI o Anthropic:
- Llama con `temperature=0` dos veces: deberías obtener la misma respuesta.
- Llama con `temperature=1.5` dos veces: serán radicalmente distintas.

---

## 📎 Para profundizar
- 📝 [OpenAI API Reference — temperature](https://platform.openai.com/docs/api-reference/chat/create#chat-create-temperature) — definición técnica oficial.
- 🎥 [Prompt Engineering Guide — Temperature & Top-P](https://www.promptingguide.ai/introduction/settings) — explicación visual práctica.
- 🧪 [OpenAI Playground](https://platform.openai.com/playground) — puedes mover el dial de temperatura en tiempo real y ver el efecto (requiere cuenta gratuita).
