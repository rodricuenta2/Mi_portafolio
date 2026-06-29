# Documento de Requisitos del Producto (PRD)
## Proyecto: Landing Page / Portafolio Profesional en GitHub Pages

---

### 1. Visión General del Producto
* **Objetivo:** Crear una landing page estática e impactante que sirva como portafolio profesional para mostrar proyectos, habilidades y trayectoria, facilitando que reclutadores y clientes potenciales te contacten.
* **Público Objetivo:** Reclutadores de talento (HR), Tech Leads, Project Managers y clientes freelance.
* **Alineación Técnica:** Desplegado de forma gratuita a través de **GitHub Pages**, utilizando tecnologías web estándar (HTML5, CSS3, JavaScript) o un generador de sitios estáticos (como Jekyll, Astro, o React/Vue si prefieres un framework).

---

### 2. Objetivos y Métricas de Éxito (KPIs)
* **Velocidad de Carga:** Score mayor a 90/100 en Google PageSpeed Insights (fundamental para retener visitas).
* **Conversión:** Lograr que los visitantes den clic en el botón de contacto o descarguen el CV.
* **Accesibilidad / SEO:** Cumplir con buenas prácticas (tags semánticos, alt text en imágenes) para un buen posicionamiento básico.

---

### 3. Requisitos Funcionales (Funcionalidades Clave)

El sitio se estructurará en una sola página (Single Page Application o Scroll Continuo) con las siguientes secciones:

#### 3.1. Sección Hero (Introducción)
* Un saludo claro, tu rol/profesión y una propuesta de valor corta (qué haces y cómo ayudas).
* **Llamado a la Acción (CTA) Principal:** Botón destacado para "Ver Proyectos" o "Contactame".
* *Opcional:* Una foto profesional tuya o una ilustración abstracta/tech.

#### 3.2. Sección "Sobre Mí"
* Una breve biografía que resuma tu pasión, experiencia y enfoque.
* Grid o lista de tus **Habilidades Técnicas (Skills)** organizadas por categorías (ej. Frontend, Backend, Herramientas).

#### 3.3. Sección de Proyectos (Datos de Prueba / Mock Data)
* **Objetivo actual:** Validar el diseño visual, la adaptabilidad (responsiveness) del grid y el comportamiento de los botones antes de subir proyectos reales.
* **Estructura de las Tarjetas:** Cada tarjeta simulará un entorno real con imágenes de marcador de posición (placeholders) de alta calidad, descripción del problema, tecnologías y enlaces de prueba.

A continuación se detallan los **4 proyectos ficticios** que poblarán la UI:

| Proyecto | Descripción / Problema Solucionado | Stack Tecnológico | Enlaces de Prueba (UI) |
| :--- | :--- | :--- | :--- |
| **1. DevTrace** | Plataforma SaaS que centraliza logs de errores en microservicios mediante dashboards interactivos en tiempo real. | React, Node.js, Tailwind CSS, WebSockets | [Demo ficticia] [GitHub repo] |
| **2. EcoMarket** | E-commerce mobile-first enfocado en productos locales con checkout optimizado en un solo paso. | Vue.js, Firebase, Stripe API, Sass | [Demo ficticia] [GitHub repo] |
| **3. FitTrack AI** | Aplicación web que utiliza inteligencia artificial local para analizar posturas de ejercicio mediante la cámara. | Vanilla JS, TensorFlow.js, HTML5 Canvas | [Demo ficticia] [GitHub repo] |
| **4. CryptoPulse** | API y panel de control que rastrea la volatilidad de tokens en mercados descentralizados con alertas por Telegram. | Python, FastAPI, PostgreSQL, Docker | [Demo ficticia] [GitHub repo] |

#### 3.4. Sección de Contacto
* Formulario de contacto funcional (integrado con servicios gratuitos como *Formspree* o *Web3Forms* ya que GitHub Pages no tiene backend).
* Enlaces directos a tus redes profesionales: **GitHub, LinkedIn** y correo electrónico.

#### 3.5. Barra de Navegación (Navbar) y Footer
* **Navbar Sticky:** Que se quede fija arriba al hacer scroll para navegar entre secciones (Sobre mí, Proyectos, Contacto).
* Botón para **Descargar CV** en formato PDF.
* **Footer:** Derechos reservados y enlaces rápidos.

---

### 4. Requisitos No Funcionales (Calidad y Técnico)

* **Responsive Design:** El diseño debe ser *Mobile-First*. Debe verse perfecto en smartphones, tablets y monitores de escritorio.
* **Performance:** Imágenes optimizadas (formatos modernos como `.webp`).
* **Despliegue Continuo (CI/CD):** Configurar GitHub Actions (o la rama `gh-pages`) para que cada vez que hagas un `git push` a `main`, el portafolio se actualice automáticamente.
* **Modo Oscuro (Opcional pero recomendado):** Un switch para cambiar entre Light/Dark mode.

---

### 5. Plan de Lanzamiento Actualizado (Fases)

* **Fase 1 (UI Sandbox & MVP):** * Construcción de la estructura completa de la Landing Page.
  * Implementación del grid de proyectos utilizando los **4 componentes de prueba** anteriores.
  * Despliegue inicial en GitHub Pages para validar que todo cargue correctamente en dispositivos móviles.
* **Fase 2 (Contenido Real):** * Reemplazo progresivo de los proyectos ficticios por tus proyectos reales a medida que los termines.
  * Integración del formulario de contacto funcional (*Formspree* / *Web3Forms*).
* **Fase 3 (Optimización):** * Animaciones de carga, Modo Oscuro y pulido de SEO.
