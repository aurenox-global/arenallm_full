# 🏟️ Arena LLM — Comparador de Modelos Open Source

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Single File](https://img.shields.io/badge/Single_File-HTML-green.svg)](index.html)
[![No Backend](https://img.shields.io/badge/No_Backend-Required-purple.svg)](#)

> **Compara 22 modelos LLM de última generación en una sola interfaz moderna.** Evalúa capacidades de codificación, razonamiento, matemáticas y más con gráficas interactivas para encontrar el modelo perfecto para tu caso de uso.

![Arena LLM Preview](https://via.placeholder.com/1200x630/0a0a0f/7c5cfc?text=Arena+LLM+Preview)

---

## ✨ Características

### 🔍 Comparación 1 vs 1
- Selecciona cualquier par de modelos y compáralos lado a lado
- Gráficos de radar para visualizar fortalezas y debilidades
- Barras comparativas por categoría (Código, Matemáticas, Razonamiento, NLP, etc.)
- Tabla detallada con diferencias puntuales

### 📊 Visualización de Datos
- **Ranking interactivo**: Top modelos por puntuación general
- **Eficiencia por parámetro**: Score normalizado por billón de parámetros
- **Análisis por familia**: Comparación entre Qwen, Llama, Gemma, Mistral, etc.
- **Scatter plot**: Relación entre parámetros y rendimiento

### 🎯 Recomendaciones Inteligentes
Sugerencias de modelos según tu caso de uso:
```
💻 Desarrollo de Software    → Qwen2.5-Coder-7B, DeepSeek-R1-Qwen-7B
🧠 Razonamiento Complejo    → DeepSeek-R1-Qwen3-8B, Qwen3-4B-Thinking
📱 Edge Computing          → SmolLM3-3B, Helium-2B, Gemma4-e2B
💬 Asistente Conversacional → Qwen3.5-9B, Mistral3-7B, Qwen3-8B
🔬 Investigación STEM      → DeepSeek-R1 series, GLM-4-9B
🌍 Multilingüe             → Qwen series, GLM-4-9B
```

### 🎨 UI/UX Moderna
- Diseño oscuro con acentos neón y efectos glassmorphism
- Animaciones suaves y micro-interacciones
- Totalmente responsive (móvil, tablet, desktop)
- Navegación por secciones con scroll suave
- Filtros por tipo de modelo (Coder, Reasoning, General, Ligero)

---

## 🤖 Modelos Incluidos (22)

### Familia Qwen
| Modelo | Parámetros | Tipo | Destacado |
|--------|-----------|------|-----------|
| Qwen2.5-3B | 3B | General | Ligero y versátil |
| Qwen2.5-7B | 7B | General | Balance excelente |
| Qwen2.5-Coder-3B | 3B | 🧑‍💻 Coder | Código eficiente |
| Qwen2.5-Coder-7B | 7B | 🧑‍💻 Coder | Top coding sub-10B |
| Qwen3-4B | 4B | General | Nueva generación |
| Qwen3-8B | 8B | General | Rendimiento superior |
| Qwen3.5-4B | 4B | General | Reasoning mejorado |
| Qwen3.5-9B | 9B | General | ⭐ Top general |
| Qwen3-4B-Thinking | 4B | 🧠 Reasoning | Chain-of-thought |

### Familia DeepSeek (R1 Distill)
| Modelo | Parámetros | Tipo | Destacado |
|--------|-----------|------|-----------|
| DeepSeek-R1-Distill-Llama-8B | 8B | 🧠 Reasoning | Razonamiento avanzado |
| DeepSeek-R1-Distill-Qwen-7B | 7B | 🧠 Reasoning | STEM especializado |
| DeepSeek-R1-0528-Qwen3-8B | 8B | 🧠 Reasoning | 🏆 Mejor reasoning |

### Familia Llama
| Modelo | Parámetros | Tipo | Destacado |
|--------|-----------|------|-----------|
| Llama3.2-3B | 3B | General | Ecosistema Meta |
| Llama3.1-8B | 8B | General | Comunidad activa |

### Familia Gemma
| Modelo | Parámetros | Tipo | Destacado |
|--------|-----------|------|-----------|
| Gemma3-4B | 4B | General | Integración Google |
| Gemma4-e2B | 2B | ⚡ Ligero | MoE ultra-eficiente |
| Gemma4-e4B | 4B | General | MoE balanceado |

### Otros Modelos Destacados
| Modelo | Parámetros | Familia | Destacado |
|--------|-----------|---------|-----------|
| SmolLM3-3B | 3B | SmolLM | ⚡ Máxima eficiencia |
| Helium-2B | 2B | Helium | 🪶 Ultra ligero |
| Phi-3.5 Mini | 3.8B | Microsoft | 🎯 Datos de calidad |
| Mistral3-7B | 7B | Mistral | 📋 Instrucciones |
| GLM-4-9B-Chat | 9B | Zhipu AI | 🌍 Bilingüe CN/EN |

---

## 🚀 Cómo Usar

### Opción 1: Ejecutar Localmente (Recomendado)
```bash
# 1. Clonar el repositorio
git clone https://github.com/tu-usuario/arena-llm.git
cd arena-llm

# 2. Abrir directamente en el navegador
open index.html
# o simplemente hacer doble clic en el archivo
```

### Opción 2: Deploy en GitHub Pages
```bash
# Habilitar GitHub Pages en Settings > Pages
# Source: Deploy from branch → main → / (root)
# Tu app estará disponible en: https://tu-usuario.github.io/arena-llm
```

### Opción 3: Servidor Local con Python
```bash
python -m http.server 8000
# Acceder a: http://localhost:8000
```

### Opción 4: Deploy en Vercel/Netlify
```bash
# Con Vercel CLI
vercel --prod

# O arrastrar la carpeta a Netlify Drop
```

---

## 🛠️ Stack Tecnológico

```
📄 Single HTML File (sin dependencias de build)
🎨 Tailwind CSS (vía CDN) - Utilidades CSS
📊 Chart.js (vía CDN) - Visualización de datos
🔤 Google Fonts - Inter & JetBrains Mono
⚡ Vanilla JavaScript - Sin frameworks pesados
🎭 CSS Custom Properties - Tema oscuro personalizable
```

### Estructura del Proyecto
```
arena-llm/
├── index.html          # Aplicación completa en un solo archivo
├── README.md           # Este archivo
├── LICENSE             # Licencia MIT
└── .github/
    └── workflows/
        └── deploy.yml  # (Opcional) Auto-deploy a GitHub Pages
```

---

## 📈 Métricas Evaluadas

Cada modelo incluye puntuaciones en 8 categorías (0-100):

| Categoría | Descripción | Peso en Overall |
|-----------|-------------|----------------|
| 💻 Código | Generación, debugging, comprensión de código | 15% |
| 🔢 Matemáticas | Resolución de problemas numéricos y algebraicos | 15% |
| 🧠 Razonamiento | Lógica, planificación, chain-of-thought | 20% |
| 💬 NLP | Comprensión de lenguaje, generación de texto | 15% |
| ⚡ Eficiencia | Velocidad de inferencia, uso de recursos | 10% |
| 📋 Instrucciones | Seguimiento de prompts, alineación | 10% |
| 🌍 Multilingüe | Soporte para múltiples idiomas | 10% |
| 🎨 Creatividad | Generación creativa, originalidad | 5% |

> ⚠️ **Nota**: Las puntuaciones son estimaciones basadas en benchmarks públicos (MT-Bench, HumanEval, GSM8K, etc.) y evaluaciones comunitarias. No reemplazan pruebas en tu caso de uso específico.

---

## 🔧 Personalización

### Agregar un Nuevo Modelo
Edita el array `models` en el `<script>` de `index.html`:

```javascript
{
    id: 'mi-modelo-7b',
    name: 'Mi Modelo 7B',
    family: 'MiFamilia',
    params: 7,
    type: 'general', // 'coder' | 'reasoning' | 'general' | 'light'
    badge: 'Nuevo',
    badgeClass: 'badge-general', // badge-coder | badge-reasoning | badge-light
    desc: 'Descripción breve del modelo...',
    highlights: 'Punto fuerte 1, punto fuerte 2',
    bestFor: 'Casos de uso recomendados',
    scores: {
        code: 65, math: 60, reasoning: 62, nlp: 70,
        efficiency: 75, instruction: 68, multilingual: 64, creativity: 55
    },
    overall: 64.9 // Promedio ponderado
}
```

### Cambiar el Tema de Colores
Modifica las variables CSS en `:root`:

```css
:root {
    --accent: #7c5cfc;      /* Color principal */
    --accent2: #5c8cfc;     /* Color secundario */
    --accent3: #fc5c8c;     /* Color de énfasis */
    --bg: #0a0a0f;          /* Fondo principal */
    --surface: #12121a;     /* Tarjetas */
    /* ... */
}
```

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! 

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -m 'feat: agregar nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

### Ideas para Contribuir
- [ ] Agregar soporte para comparar 3+ modelos simultáneamente
- [ ] Importar datos reales desde la API de Hugging Face
- [ ] Añadir modo "Batalla Aleatoria" para descubrimiento
- [ ] Exportar resultados de comparación a JSON/PDF
- [ ] Traducciones a otros idiomas (i18n)
- [ ] Modo accesibilidad (alto contraste, screen readers)

---

## ⚠️ Descargo de Responsabilidad

> Este proyecto es una herramienta de **comparación educativa y orientativa**. 
> 
> - Las puntuaciones no son oficiales ni certificadas
> - El rendimiento real depende de tu hardware, configuración y caso de uso específico
> - Los modelos listados son propiedad de sus respectivos creadores (Alibaba, Meta, Google, Mistral, Zhipu AI, Microsoft, etc.)
> - Este proyecto no está afiliado con ninguna de las organizaciones mencionadas
> - Siempre verifica los términos de uso y licencias de cada modelo antes de usarlo en producción

---

## 📄 Licencia

Distribuido bajo la licencia **MIT**. Ver [`LICENSE`](LICENSE) para más información.

```
MIT License

Copyright (c) 2024 Arena LLM Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 Agradecimientos

- 🤗 [Hugging Face](https://huggingface.co) por democratizar el acceso a modelos open source
- 📊 Comunidades de benchmarks: [HELM](https://crfm.stanford.edu/helm/), [Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)
- 🎨 Inspiración de diseño: [Vercel](https://vercel.com), [Linear](https://linear.app), [Raycast](https://raycast.com)
- ⚡ Librerías: [Tailwind CSS](https://tailwindcss.com), [Chart.js](https://www.chartjs.org)

---

## 📬 Contacto

¿Preguntas, sugerencias o bugs? 
- 🐛 [Abre un Issue](https://github.com/tu-usuario/arena-llm/issues)
- 💬 [Discussions](https://github.com/tu-usuario/arena-llm/discussions)
- ✉️ tu-email@ejemplo.com

---

<div align="center">

**⭐ Si te gusta este proyecto, ¡dale una estrella en GitHub!**

*Hecho con ❤️ para la comunidad open source de IA*

</div>
