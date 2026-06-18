# Railytics Mobile 🚂📊

**Railytics Mobile** es una aplicación móvil nativa para Android diseñada para el monitoreo, seguimiento y análisis en tiempo real de transmisiones ferroviarias en vivo (principalmente cámaras web de *Virtual Railfan* en EE. UU.).

La aplicación integra una potente interfaz híbrida web-nativa para procesar analíticas avanzadas, mostrar métricas en tiempo real de detección de trenes, y proporcionar un registro histórico visual de eventos ferroviarios.

---

## 🚀 Características Principales

### 1. Monitoreo y Selección de Transmisiones (Streams)
* **Visualización Multi-Stream:** Permite monitorear cámaras ferroviarias activas de múltiples ubicaciones (ej. Kearney, Nebraska; Fairport, Nueva York; Folkston, Georgia; Fort Madison, Iowa; Lincoln, Nebraska; Chehalis, Washington; Glendale, Ohio; entre otras).
* **Control Centralizado:** Permite iniciar o detener el análisis de todas las transmisiones de forma simultánea.

### 2. Panel de Análisis en Tiempo Real (Real-Time Analytics)
* **Métricas de Rendimiento:** Velocidad de procesamiento en cuadros por segundo (FPS).
* **Ranking de Transmisiones:** Top 5 de cámaras con mayor actividad de detección.
* **Salud del Sistema:** Monitoreo del estado simulado de CPU, memoria y red.
* **Visualización de Datos Dinámica:**
  * Gráfico de líneas con métricas de rendimiento en tiempo real.
  * Gráfico de área apilada para tendencias de detección acumuladas.
  * Gráfico de barras comparativo de detecciones entre diferentes locaciones.
  * Gráfico de pastel (pie chart) con la tasa de detección por transmisión.
  * Mapa de calor (Heatmap) de actividad horaria diaria.
* **Alertas y Eventos en Vivo:** Canal de notificaciones y alertas instantáneas en pantalla ante nuevas detecciones.
* **Línea de Tiempo (Timeline):** Cronología vertical con las detecciones más recientes.

### 3. Registro Histórico y Calendario
* **Calendario de Eventos:** Interfaz interactiva de calendario para explorar registros anteriores, con opciones de filtrado rápido por ubicación geográfica.
* **Detalle por Sesión:** Desglose del progreso del análisis de cada cámara, incluyendo el conteo de fotogramas procesados, trenes detectados y fotogramas descartados.

### 4. Galería de Fotogramas (Frame Gallery)
* Captura y visualización de imágenes (frames) de los trenes detectados, organizados por locación con paginación integrada.

### 5. Resiliencia de Conexión (Offline Support)
* La aplicación cuenta con una pantalla de error nativa en **Jetpack Compose** que detecta la pérdida de conexión a internet, previniendo pantallas en blanco y permitiendo al usuario reintentar la carga de la aplicación fácilmente.

---

## 🛠️ Tecnologías Utilizadas

* **Móvil (Android):**
  * **Kotlin** para la lógica de la aplicación nativa.
  * **Jetpack Compose** para el diseño de la interfaz de usuario nativa y el control del estado de error y conexión.
  * **WebView & WebViewAssetLoader:** Integración segura y eficiente para cargar recursos locales en el WebView de Android sin depender de peticiones HTTP externas.
* **Frontend Web (Híbrido):**
  * **HTML5 y CSS3** (diseño oscuro dinámico con detalles en color amarillo corporativo `#FFAD01` y `#FFC107`).
  * **JavaScript (ES6)** para la interactividad y la simulación del motor de telemetría y analíticas.
  * **Chart.js v4.4.7** para la generación interactiva y animada de gráficos avanzados.
  * **Material Icons & Google Fonts (Roboto):** Para una tipografía moderna y elementos visuales estandarizados.

---

## 📂 Estructura del Proyecto

* [MainActivity.kt](file:///c:/Users/Felip/AndroidStudioProjects/Railyticsmobile/app/src/main/java/com/autonovations/railytics_mobile/MainActivity.kt): Punto de entrada nativo de la app. Administra el estado de la conexión, el cargador de recursos locales (`WebViewAssetLoader`) y renderiza la vista.
* [railytics.html](file:///c:/Users/Felip/AndroidStudioProjects/Railyticsmobile/app/src/main/assets/railytics.html): Código principal que contiene el diseño de la app, los gráficos, y el motor de telemetría/simulación de eventos.
* `Railytics/`: Carpeta con copias de respaldo de los recursos del frontend.

---

## 📦 Compilación y Ejecución

1. Abre el proyecto en **Android Studio**.
2. Sincroniza el proyecto con Gradle (`settings.gradle.kts` y `build.gradle.kts`).
3. Conecta un dispositivo físico o inicia un emulador Android.
4. Ejecuta la aplicación utilizando la configuración estándar `app`.

---

## 📝 Licencia

Este proyecto es propiedad de **Autonovations** en colaboración con **Union Pacific (UP)**.
