# Embeddings

> **En una oración:** Son números que representan el significado de un texto, permitiendo que la IA busque por similitud de ideas, no por palabras exactas.

---

## ¿Qué es?
Un embedding es la transformación de un texto (palabra, frase, párrafo) en una lista de números — un vector en un espacio matemático de cientos o miles de dimensiones. Textos con significados similares quedan cerca en ese espacio; textos con significados distintos quedan lejos.

Esto es lo que hace posible la búsqueda semántica: si buscas "cómo mejorar mis ventas", el sistema puede encontrar documentos que hablan de "estrategias comerciales" o "aumentar conversiones" aunque ninguno de esos documentos use exactamente esas palabras.

Es la tecnología central detrás de RAG, de los motores de búsqueda modernos y de los sistemas de recomendación.

---

## Analogía
Imagina un **mapa donde los países con culturas similares están cerca geográficamente**. Francia y España quedan cerca; Japón y Corea quedan cerca; pero Francia y Japón quedan lejos. Los embeddings hacen lo mismo con el significado: "perro" y "mascota" quedan cerca en el mapa; "perro" y "logaritmo" quedan muy lejos.

---

## 🧪 Pruébalo
**Opción 1 (visual, sin código):**
Ve a [projector.tensorflow.org](https://projector.tensorflow.org) — es una visualización 3D de embeddings reales. Escribe palabras y observa cuáles quedan cerca entre sí.

**Opción 2 (con código, 5 minutos):**
```python
# Instala: pip install sentence-transformers
from sentence_transformers import SentenceTransformer, util

model = SentenceTransformer('all-MiniLM-L6-v2')

frases = ["El perro corre en el parque", "El can trota por el jardín", "La inflación subió un 3%"]
embeddings = model.encode(frases)

similitud = util.cos_sim(embeddings[0], embeddings[1])
print(f"Similitud frase 1 y 2: {similitud.item():.2f}")  # debería ser alta (~0.85)
similitud2 = util.cos_sim(embeddings[0], embeddings[2])
print(f"Similitud frase 1 y 3: {similitud2.item():.2f}")  # debería ser baja (~0.1)
```

**¿Qué observar?** Las dos frases sobre el perro tienen alta similitud aunque no comparten casi ninguna palabra. La frase sobre inflación tiene similitud casi nula. Eso es el poder del significado codificado en números.

---

## 📎 Para profundizar
- 🎥 [3Blue1Brown — "Transformers (how LLMs work)"](https://www.youtube.com/watch?v=wjZofJX0v4M) — el mejor video visual sobre cómo el modelo construye representaciones de significado.
- 🔧 [TensorFlow Embedding Projector](https://projector.tensorflow.org) — visualización interactiva sin código.
- 📝 [Hugging Face — Sentence Transformers](https://www.sbert.net) — librería y documentación para usar embeddings en tus propios proyectos.
