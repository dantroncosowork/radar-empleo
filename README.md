# 📡 Radar de Empleo & AI Career Coach · Demo Técnica

> Interfaz interactiva, análisis de encaje profesional y asistente de postulación inteligente para el sector tecnológico y de operaciones.  
> Diseñado como una aplicación web autónoma de un solo archivo (sin frameworks pesados ni dependencias externas), con datos estructurados y generación asistida por IA.

🔗 **[Acceder a la Demo en Vivo (GitHub Pages)](https://dantroncosowork.github.io/radar-empleo/)**

---

## 💡 Sobre el Proyecto

Este proyecto nació para solucionar un problema real: muchas ofertas en portales de empleo tradicionales tienen títulos engañosos (p. ej., vacantes tituladas *"Analista Funcional"* que en la descripción exigen 5 años programando microservicios en Java), requisitos desmedidos o condiciones no alineadas con la energía y estilo de trabajo del candidato.

Para resolverlo, construí un sistema integral de dos componentes:
1. **Un motor de exploración y cribado en segundo plano (Python + Gemini API):** Ingesta alertas y vacantes remotas, ejecuta una criba algorítmica de Fase 1 para eliminar ruido a coste cero y evalúa las vacantes candidatas extrayendo su descripción web completa con modelos de lenguaje.
2. **Un Dashboard Interactivo (esta demo pública):** Una interfaz web de alta fidelidad visual en un único archivo HTML/CSS/JS que organiza los hallazgos en un embudo claro, compara rutas de carrera y genera cartas de presentación adaptadas en un solo clic.

---

## 🚀 Funcionalidades Principales de la Demo

### 1. 🎯 Embudo de Selección Semanal (Funnel)
* Monitorización visual del flujo completo: volumen total procesado (correo + APIs web), descartes algorítmicos en Fase 1, candidatas analizadas con IA y ofertas finalistas de alto encaje.
* Métricas transparentes de conversión semanal para medir la calidad del radar.

### 2. 💼 Tarjetas de Ofertas con Encaje Calibrado
* Clasificación por áreas profesionales: **Área A** (Soporte & CX), **Área B** (Fintech / Operaciones), **Área C** (IA sin código / Anotación y Evaluación de LLMs) y **Área D** (Producto / Operaciones técnicas).
* Identificación automática de *ofertas trampolín* (posiciones de entrada rápida para ganar experiencia corporativa y saltar a roles de mayor valor).
* Filtros interactivos instantáneos por área, modalidad remota y nivel de encaje.

### 3. ✍️ Generador y Visualizador de Cartas de Presentación
* Cada vacante analizada incluye una **carta de presentación personalizada pregenerada con IA** orientada a destacar experiencia real, habilidades transferibles y métricas tangibles (sin clichés genéricos).
* **Modal interactivo con 3 enfoques:**
  * *Original:* Equilibrado y directo.
  * *IA & Automatización:* Destaca prompting, flujos con herramientas modernas y evaluación de modelos.
  * *Operaciones & CX:* Enfocado en soporte técnico bilingüe, resolución de incidencias y métricas de servicio.
* Función de copiado al portapapeles en 1 clic y **redactor libre** para pegar cualquier oferta externa y generar una propuesta a medida.

### 4. 🧭 Matriz Comparativa de Caminos de Carrera
* Comparador dinámico de **5 rutas profesionales realistas** a 4 años:
  1. *Automatización IA & Operaciones* (De operador de herramientas a consultor de sistemas).
  2. *Diseño de Interfaces & Design Engineer* (Creación de software funcional con IA).
  3. *Analista de Datos → Data Science* (Ruta escalonada desde BI corporativo).
  4. *QA & Testing de Aplicaciones* (Control de calidad y testing asistido).
  5. *Soporte Bilingüe → Support Ops* (Uso de idiomas como trampolín hacia operaciones).
* **Radiografía técnica por ruta:** Stack demandado, densidad de estudio (1-10), exigencia matemática, lógica, carga social y marketing personal.
* **Testimonios del sector:** pros y contras de cada ruta, resumidos de lo que cuentan profesionales en foros como Reddit.

### 5. 🤖 Perfil Estratégico & Recomendaciones del Mentor
* Diagnóstico de balance de energía, arquetipo de trabajo y directrices para maximizar la productividad sostenible.
* Plan de acción semanal priorizado en 3 bloques concretos (<5h): Empleo, Formación y Portafolio.

---

## 🛠️ Stack y Arquitectura Técnica

| Capa | Tecnologías | Propósito |
|---|---|---|
| **Frontend UI** | HTML5 semántico, CSS3 moderno (Custom Properties, OKLCH, Grid/Flexbox), Vanilla JavaScript (ES6+) | Interfaz ultra-rápida, responsive, autocontenida en un único archivo sin bundlers ni frameworks pesados (0 KB dependencias externas). |
| **Diseño** | Tema *Midnight Emerald*, tipografías Inter y JetBrains Mono, paleta de alto contraste para lectura técnica prolongada. | Estética inspirada en herramientas profesionales de operaciones y terminales financieras. |
| **Motor de IA** | Google Gemini API (modelos Flash y Flash-Lite con structured prompting) | Clasificación semántica de ofertas, descarte de requisitos engañosos y redacción persuasiva de cartas. |
| **Pipeline de Automatización** | Python 3, Regex parsing, BeautifulSoup, scripts de inyección JSON y Cron/Sidecars autónomos | Lectura de fuentes, normalización de datos y sincronización periódica del dashboard. |

---

## 📂 Estructura de este Repositorio

```text
├── index.html       # Aplicación interactiva completa (HTML + CSS + JS + Dataset mock)
├── .nojekyll        # Configuración para despliegue directo en GitHub Pages
├── .gitignore       # Exclusiones de control de versiones
└── README.md        # Documentación técnica del proyecto
```

---

## 🔒 Privacidad y Datos Mock

Esta versión pública está construida sobre un **candidato inventado** («Alex») y **empresas ficticias** (Contoso, Fabrikam, Woodgrove…). Las ofertas, las cartas, el perfil y el plan semanal son de muestra, y los enlaces de las ofertas llevan a la portada de cada portal (Himalayas, InfoJobs), no a vacantes concretas. El panel real funciona igual, pero con datos propios que no se publican. No contiene correos, tokens ni claves de API.

---

## 👤 Autor

**Daniel Troncoso**  
* Explorador de herramientas con IA, automatización de procesos y diseño de software funcional.  
* GitHub: [@dantroncosowork](https://github.com/dantroncosowork)  
* Portafolio: [portafoliodanieltroncoso.vercel.app](https://portafoliodanieltroncoso.vercel.app)

---

*Desarrollado mediante pair-programming asistido con modelos avanzados de inteligencia artificial (Antigravity & Gemini).*
