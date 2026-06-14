# Rol (Role Prompting)

> **En una oración:** Es decirle a la IA qué personaje o experto debe interpretar para que sus respuestas sean más útiles y enfocadas.

---

## ¿Qué es?
Cuando le dices a un LLM "actúa como un médico", "eres un abogado especialista en contratos" o "eres un maestro de primaria explicando física", estás haciendo role prompting. El modelo adapta su vocabulario, nivel de detalle, tono y perspectiva para alinearse con ese rol.

No es magia — es que el modelo fue entrenado con millones de textos escritos por personas en esos roles. Al asignarle uno, activa patrones de lenguaje y conocimiento asociados a ese perfil.

**Importante:** El rol no le da al modelo información que no tiene, pero sí cambia cómo organiza y presenta lo que sí sabe.

---

## Analogía
Es como pedirle a un actor versátil que interprete a un personaje específico. El actor sigue siendo el mismo (el modelo base), pero ajusta su manera de hablar, sus referencias y su enfoque según el papel que le asignaste.

---

## 🧪 Pruébalo
Haz la misma pregunta con tres roles distintos:

> **Pregunta:** "Explícame qué es la inflación."

1. Sin rol: solo hazla así.
2. Con rol de economista: `"Actúa como un economista del Banco Mundial. Explícame qué es la inflación."`
3. Con rol de maestro: `"Actúa como un maestro de primaria. Explícame qué es la inflación para niños de 10 años."`

**¿Qué observar?** Tres respuestas radicalmente distintas con exactamente la misma pregunta base. El rol es el contexto que calibra todo lo demás.

---

## 📎 Para profundizar
- 📝 [Anthropic — Role prompting](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/use-a-role) — guía oficial con ejemplos reales.
- 📝 [Prompt Engineering Guide — Role Prompting](https://www.promptingguide.ai/techniques/zeroshot#role-prompting) — comparativa de técnicas.
- 🧪 [PromptBase](https://promptbase.com) — marketplace de prompts reales donde puedes ver cómo distintos roles se estructuran en la práctica.
