# 🎓 EduSteam

**EduSteam** es una plataforma web diseñada para conectar estudiantes con tutores verificados, facilitando el aprendizaje personalizado a través de sesiones virtuales en tiempo real.

---

## 📌 Descripción general

EduSteam permite a los estudiantes encontrar al tutor ideal según la materia que necesitan reforzar, agendar sesiones, comunicarse directamente con sus tutores y llevar un seguimiento de su progreso académico. Todo desde una interfaz moderna, intuitiva y coherente visualmente.

---

## 🗂️ Estructura de pantallas

El proyecto está compuesto por las siguientes páginas:

| Archivo | Descripción |
|---|---|
| `index.html` | Página de inicio / Landing page |
| `buscar_tutores.html` | Buscador y listado de tutores disponibles |
| `perfil_usuario.html` | Perfil detallado de un tutor |
| `agendar_sesion.html` | Calendario para agendar una sesión con un tutor |
| `mensajes.html` | Chat en tiempo real entre estudiante y tutor |
| `progreso.html` | Dashboard de progreso académico del estudiante |
| `sesion.html` | Pantalla de videollamada durante una sesión en vivo |

---

## 📄 Descripción de cada pantalla

### 🏠 `index.html` — Inicio
Página principal de bienvenida. Presenta el slogan de la plataforma, una imagen hero, el botón principal para encontrar un profesor y una fila de estadísticas clave (satisfacción, estudiantes ayudados, tutores verificados y clases realizadas).

### 🔍 `buscar_tutores.html` — Nuestros Maestros
Listado de tutores con buscador en tiempo real y chips de filtro por materia o especialidad. Cada tarjeta muestra nombre, materia, descripción breve, calificación y precio por hora.

### 👤 `perfil_usuario.html` — Perfil del tutor
Vista detallada de un tutor específico. Incluye foto, descripción, materias, reseñas de otros estudiantes, video de presentación y botones para enviar mensaje o contratar al tutor.

### 📅 `agendar_sesion.html` — Agendar sesión
Calendario interactivo donde el estudiante selecciona el día disponible y el horario deseado. Muestra un resumen de la reserva con tutor, fecha, hora y precio total. Al confirmar, aparece un modal de confirmación centrado.

### 💬 `mensajes.html` — Mensajes
Pantalla de chat dividida en tres columnas: lista de tutores activos, conversación central con burbujas diferenciadas (tutor y estudiante), y panel lateral con los materiales recibidos (PDFs, imágenes) y acceso a la próxima sesión.

### 📊 `progreso.html` — Mi Progreso
Dashboard con métricas del estudiante: sesiones completadas, horas de tutoría, temas reforzados y mejora en calificaciones. Incluye barras de progreso por materia y un gráfico de barras con la evolución de notas promedio por mes. Al final muestra retroalimentación reciente de cada sesión.

### 🎥 `sesion.html` — Sesión en vivo
Pantalla de videollamada con vista principal del estudiante, miniatura PiP (picture-in-picture) del tutor, barra de controles (micrófono, cámara, compartir pantalla, chat, participantes) y botón de colgar con modal de confirmación para salir.

---

## 🎨 Tecnologías y estilos

- **HTML5** semántico
- **CSS3** — Variables de color, Grid, Flexbox, animaciones y transiciones
- **JavaScript** vanilla — Sin frameworks externos
- **Google Fonts** — Tipografías `El Messiri` (títulos) e `Inter` (cuerpo)
- **SVG** inline para todos los íconos

### Paleta de colores principal

| Rol | Color |
|---|---|
| Primario (navy) | `#1a2356` |
| Acento púrpura | `#9176AB` |
| Lavanda claro | `#c7bfe8` |
| Fondo general | `#f0f2f7` |
| Texto secundario | `#6b7280` |

---

## 🗃️ Archivos CSS y JS

Cada pantalla tiene su propio archivo CSS y JS adicional que **no modifica** el código base, solo lo extiende:

| Pantalla | CSS adicional | JS adicional |
|---|---|---|
| Mensajes | `mensajes.css` | `mensajes.js` |
| Progreso | `progreso.css` | `progreso.js` |
| Sesión en vivo | `sesion.css` | `sesion.js` |
| Agendar sesión | *(incluido en el HTML)* | *(incluido en el HTML)* |

El archivo base `style.css` y `script.js` son compartidos por todas las páginas.

---

## 📁 Estructura de carpetas recomendada

```
edusteam/
│
├── index.html
├── buscar_tutores.html
├── perfil_usuario.html
├── agendar_sesion.html
├── mensajes.html
├── progreso.html
├── sesion.html
│
├── style.css
├── script.js
│
├── mensajes.css
├── mensajes.js
├── progreso.css
├── progreso.js
├── sesion.css
├── sesion.js
│
├── images/
│   ├── logo.png
│   ├── chico_estudiando.jpeg
│   ├── profesora.png
│   └── estudiante_en_sesion.png
│
└── README.md
```

---

## ✨ Funcionalidades destacadas

- 🔎 **Búsqueda en tiempo real** de tutores por nombre, materia o etiqueta
- 📅 **Calendario interactivo** con días disponibles resaltados y selección de horario
- 💬 **Chat con envío de mensajes** y soporte para archivos adjuntos (PDFs)
- 📊 **Animaciones de entrada** en barras de progreso y contadores numéricos
- 🎥 **Videollamada** con controles de micrófono, cámara y pantalla compartida
- 🔔 **Modales de confirmación** para acciones críticas (reserva, salir de sesión)
- 📱 **Diseño responsive** con breakpoints para tablet y móvil

---

## 🚀 Cómo ejecutar el proyecto

1. Clona o descarga el repositorio.
2. Coloca todas las imágenes en la carpeta `/images/`.
3. Abre `index.html` en tu navegador (sin necesidad de servidor).
4. Para una mejor experiencia, usa un servidor local como **Live Server** en VS Code.

> ⚠️ Algunas funcionalidades como la cámara o el micrófono real en `sesion.html` requieren contexto HTTPS o `localhost`.

---

## 👥 Equipo

Proyecto desarrollado como parte de una plataforma educativa para conectar estudiantes con tutores de calidad en materias STEAM.

---

*EduSteam — La forma más fácil de encontrar un buen tutor* 🧠
