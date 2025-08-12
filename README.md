# Desglose de Fases y Cumplimiento

## Fase 1: Configuración del Entorno y Planificación

- **Creación del Repositorio:**
	- El repositorio fue creado en GitHub: [examen-integrativa-U3](https://github.com/DarwinToapanta01/examen-integrativa-U3.git)
- **Estructura de Archivos:**
	- Se definió una estructura lógica con carpetas `css/`, `js/`, `assets/icons/` y archivos principales (`index.html`, `manifest.json`, `sw.js`, `package.json`).
- **Selección de Componentes:**
	- Inicialmente se consideró usar una librería de Web Components externa, pero se optó por Material Design Lite (MDL) para cumplir con los requisitos visuales y de interfaz.
- **Configuración Inicial:**
	- El archivo `index.html` enlaza correctamente los archivos CSS y JS, y se importan los recursos de MDL desde CDN.

## Fase 2: Desarrollo de la Interfaz y Contenido

- **Construcción de la UI:**
	- Todas las secciones (Inicio, Sobre la ESPE, Oferta Académica, Proceso de Admisión, Contacto) fueron implementadas usando componentes de Material Design Lite (cards, navbar, listas, botones).
- **Poblar Contenido:**
	- El contenido informativo de cada sección se agregó en el archivo `index.html`, asegurando legibilidad y presentación profesional.
- **Navegación:**
	- La navegación entre secciones se implementó en `js/app.js` usando el menú/header de MDL, permitiendo cambiar de sección sin recargar la página.

## Fase 3: Implementación de Funcionalidades PWA

- **Web App Manifest (`manifest.json`):**
	- El archivo contiene `name`, `short_name`, `start_url`, `display: 'standalone'`, `background_color`, `theme_color` y los iconos necesarios. Está enlazado en `index.html`.
- **Service Worker (`sw.js`):**
	- El archivo define el evento `install` para cachear todos los recursos críticos (HTML, CSS, JS, imágenes, iconos).
	- El evento `fetch` implementa la estrategia "Cache First" para servir la app offline.
- **Registro del Service Worker:**
	- El registro se realiza desde `js/app.js` al cargar la aplicación.

Cada uno de estos pasos está documentado y reflejado en los archivos fuente del proyecto, cumpliendo con los objetivos de la evaluación.

# ESPE PWA: Portal Informativo

Aplicación web progresiva (PWA) informativa sobre la Universidad de las Fuerzas Armadas ESPE, desarrollada con Material Design Lite y funcionalidades offline.

## Objetivo

Brindar información clara y accesible sobre la ESPE, sus carreras, proceso de admisión y contacto, con una interfaz moderna, instalable y funcional sin conexión.

## Secciones

- **Inicio:** Bienvenida y acceso visual a la universidad.
- **Sobre la ESPE:** Historia, misión y visión institucional.
- **Oferta Académica:** Detalle de carreras y contactos de directores.
- **Proceso de Admisión:** Pasos y requisitos para postular.
- **Contacto:** Información de contacto y ubicación.

## Tecnologías y Librerías

- Material Design Lite (MDL) para la interfaz.
- Service Worker para funcionalidad offline.
- Manifest PWA y archivos de iconos personalizados.

## Estructura del Proyecto

```
├── assets/icons/         # Iconos e imágenes (incluye espe.png)
├── css/styles.css        # Estilos personalizados
├── js/app.js             # Lógica principal y navegación
├── index.html            # Página principal y estructura UI
├── manifest.json         # Manifiesto PWA
├── sw.js                 # Service Worker
└── package.json          # Scripts y dependencias
```

## Funcionalidades PWA

- Instalación en dispositivos (botón Instalar PWA).
- Navegación entre secciones sin recargar la página.
- Acceso offline a todo el contenido y recursos.
- Iconos e imagen institucional personalizados.

## Cómo ejecutar el proyecto

```bash
# Clonar el repositorio
git clone https://github.com/DarwinToapanta01/examen-integrativa-U3.git

# Instalar dependencias
npm install

# Iniciar en modo desarrollo
npm start

```

## Despliegue

El proyecto está listo para ser desplegado en GitHub Pages como aplicación web estática.

## Autor

Darwin Toapanta

---
🔗 **GitHub:** [examen-integrativa-U3](https://github.com/DarwinToapanta01/examen-integrativa-U3.git)

---