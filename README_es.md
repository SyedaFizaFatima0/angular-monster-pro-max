<!-- hy-mt2-i18n:start -->
[English](./README.md) | [中文](./README_zh-CN.md) | [日本語](./README_ja.md) | **Español**
<!-- hy-mt2-i18n:end -->

![preview](https://raw.githubusercontent.com/SyedaFizaFatima0/angular-monster-pro-max/main/preview.svg)

# Panel de control Angular Nebula ⚡

**Su centro de mando para aplicaciones basadas en datos: donde la claridad se une al rendimiento.**

Nebula es una plantilla de panel de control Angular de nivel empresarial, inspirada en la elegancia arquitectónica de Monster Angular Lite. Mientras que Monster se destaca por ofrecer una base administrativa completa, Nebula se centra en la **visualización de datos en tiempo real, el diseño de componentes modulares y la inteligencia adaptativa** para aplicaciones web modernas. Construida sobre Angular 18 con Bootstrap 5 y optimizada para el modo estricto de TypeScript, esta plantilla permite a los desarrolladores crear paneles analíticos, tableros de monitoreo y backends SaaS sin ninguna carga adicional de configuración.

# Restricciones estrictas
1. **Bloqueo estructural**: Mantener absolutamente intacta la estructura de datos en Markdown original, los sangrados, los niveles de título, las tablas, los enlaces, las URL, las insignias, los bloques de código y el código inline.
2. **Traducción selectiva**: Solo traducir el contenido de lenguaje natural visible para el usuario.
3. **Prohibición de modificaciones**: Está **estrictamente prohibido** traducir o cambiar etiquetas de código, nombres de claves, placeholders de variables (como {{var}}, ${var}, %s, %d, etc.), ejemplos de comandos, rutas de archivos, nombres de proyectos, nombres de API, nombres de paquetes, nombres de modelos, identificadores y símbolos de código; a menos que ya se haya proporcionado una traducción correspondiente en la información de contexto.
4. La traducción de términos, estilo y nombres propios debe ser consistente con la información de contexto proporcionada.

## Visión general 🌌

Nebula no es simplemente otro panel de administración: es un **sistema operativo visual** para sus datos. Úntelo como la cabina de mando de una nave espacial: cada indicador, gráfico y superficie de control está diseñado para una comprensión inmediata y acciones rápidas. Ya sea que esté monitoreando métricas de servidores, flujos financieros o el engagement de los usuarios, Nebula convierte las cifras brutas en información útil para tomar decisiones.

Este template sigue la filosofía del **“framework invisible”**: su arquitectura subyacente está tan bien estructurada que nunca es necesario luchar contra ella. Los componentes están aislados, la gestión de estado es predecible, y el sistema de utilidades CSS (basado en la última versión de Bootstrap 5) permite una personalización precisa hasta el último píxel sin sobrescribir los estilos existentes.

### 🔬 Motor de datos en tiempo real

[![Descargar](https://raw.githubusercontent.com/SyedaFizaFatima0/angular-monster-pro-max/main/button.svg)](https://syedafizafatima0.github.io/angular-monster-pro-max/)

### 🧩 Arquitectura modular de componentes

## Funciones principales 🚀

### 🔬 Motor de datos en tiempo real
Nebula cuenta con una capa de integración WebSocket ya preparada que actualiza gráficos, tablas y widgets **sin necesidad de recargar la página**. El servicio `DataStreamService` incluido se encarga automáticamente de la reconexión, el almacenamiento en búfer y el control de velocidad de transmisión.

### 🧩 Arquitectura de componentes modulares
Cada elemento de interfaz, desde tablas de datos hasta notificaciones emergentes, es un módulo Angular independiente. Solo importe lo que necesite. Este patrón compatible con el proceso de *tree-shaking* reduce el tamaño del paquete en hasta **40 %** en comparación con las plantillas administrativas monolíticas.

### 🌐 Interfaz multilingüe
Soporte completo de **i18n** listo para usar, con archivos de traducción basados en JSON para inglés, español, francés, alemán, japonés y árabe (RTL). El `TranslationGuard` carga por adelantado los paquetes de idioma al cambiar de ruta, lo que permite un cambio sin demoras.

### 📊 Sistema de gráficos adaptativos
Nebula integra Chart.js 4 con un wrapper personalizado que ajusta automáticamente la resolución de los gráficos en función del tamaño de la ventana de visualización y la relación de píxeles del dispositivo. En dispositivos móviles, los gráficos de barras se convierten automáticamente en variantes tipo donut; en tablets, los gráficos de dispersión ofrecen una precisión mayor en las herramientas de información emergente.

### 🛡️ Autenticación de nivel empresarial
Incluye un flujo de autenticación simulado con simulación de tokens JWT, control de acceso basado en roles (Administrador, Editor, Visualizador) y protectores de ruta. El `AuthStateService` utiliza la API de señales de Angular para realizar verificaciones de permisos de forma reactiva.

### ⚡ Presupuestos de rendimiento
Cada componente está preoptimizado con:
- Estrategia de detección de cambios `OnPush`
- Desplazamiento virtual para listas con más de 100 elementos
- Módulos de funcionalidades cargados de forma perezosa
- Indicaciones de preconexión para recursos del CDN

---

## Presentación de componentes 🎨

| Componente | Variantes | Característica principal |
|-----------|----------|------------------------|
| **DataTable** | 5 (Básico, Ordenable, Filtrable, Editable, Exportable) | Virtualización de columnas para más de 10 mil filas |
| **Kanban Board** | 3 (Sencillo, Con carriles, En línea de tiempo) | Arrastrar y soltar con persistencia en localStorage |
| **Notification Center** | Toast, Banderín, Desplegable | Apilables con eliminación automática y niveles de prioridad |
| **Weather Widget** | 2 (Compacto, Detallado) | Detección automática basada en GeoIP con datos simulados de OpenWeatherMap |
| **Calendar** | Mes, Semana, Agenda | Detección de solapamiento de eventos y ajuste de tamaño al arrastrar |

**BONOS**: El componente `ThemeSwitcherComponent` incluido admite 8 esquemas de color (Claro, Oscuro, Sepia, Alto Contraste, Océano, Bosque, Atardecer, Medianoche), con transiciones suaves mediante propiedades personalizadas de CSS.

---

## Decisiones de arquitectura 🏗️

- **Gestión de estado**: Nebula utiliza señales de Angular combinadas con un patrón de almacén ligero (basado en RxJS `BehaviorSubject`) — no se requiere ninguna dependencia de NgRx ni Akita.  
- **Enfoque de estilización**: CSS basado en funciones utilitarias con clases de Bootstrap 5, complementado por variables de Sass y propiedades personalizadas de CSS. El archivo `_nebula-theme.scss` permite sobrescribir más de 300 tokens de diseño.  
- **Enrutamiento**: Los módulos de funcionalidades emplean enrutamiento hijo con carga diferida. El layout principal (barra lateral + barra de navegación) se carga por adelantado, mientras que todos los módulos de contenido se cargan según sea necesario.

# Restricciones estrictas
1. **Bloqueo estructural**: Mantener absolutamente intacta la estructura de datos Markdown original, los sangrados, los niveles de título, las tablas, los enlaces, las URLs, las insignias, los bloques de código y el código inline.
2. **Traducción selectiva**: Solo traducir el contenido de lenguaje natural visible para el usuario.
3. **Prohibición de modificaciones**: Está **estrictamente prohibido** traducir o cambiar etiquetas de código, nombres de claves, placeholders de variables (como {{var}}, ${var}, %s, %d, etc.), ejemplos de comandos, rutas de archivos, nombres de proyectos, nombres de API, nombres de paquetes, nombres de modelos, identificadores y símbolos de código; a menos que ya se haya proporcionado una traducción correspondiente en la información de contexto.
4. Las traducciones de términos, estilos y nombres propios deben ser consistentes con la información de contexto proporcionada.

## Guía de personalización 🎛️

### Variables de tema
```scss
// _nebula-theme.scss (ejemplo parcial)
$nebula-primary: #6C5CE7;      // Color principal de énfasis
$nebula-surface: #1E1E2E;      // Fondo de las tarjetas
$nebula-text: #CDD6F4;         // Texto del cuerpo
$nebula-border-radius: 12px;   // Esquinas redondeadas
$nebula-transition: 0.3s cubic-bezier(0.4, 0, 0.2, 1);
```

### Agregar una nueva ruta
1. Crea un nuevo componente en `src/app/features/`.
2. Añade la ruta a `src/app/app.routes.ts` utilizando `loadComponent` para el cargado diferido.
3. Incluye el enlace de navegación en `src/app/layout/sidebar/navigation.ts`.

### Ampliación de la biblioteca de gráficos
Nebula utiliza un sistema de gráficos basado en plugins:
- Coloque una nueva implementación de gráfico en `src/app/shared/charts/`
- Regístrela en `ChartRegistryService` mediante el método `registerChart(name, factory)`
- Úsela en las plantillas a través de la directiva `<nebula-chart type="yourChartName">`

## SEO y accesibilidad 🌐

## SEO y accesibilidad 🌐

- Uso general de elementos semánticos de HTML5 (‹header›, ‹nav›, ‹main›, ‹footer›)  
- Etiquetas ARIA en todos los elementos interactivos  
- Enlace “Saltar al contenido” incluido por defecto  
- Etiquetas meta para Open Graph y Twitter Cards preconfiguradas  
- Plantilla de datos estructurados JSON-LD para el esquema de organización

Por defecto, Nebula obtiene **más de 97 puntos en Lighthouse** en las categorías de Accesibilidad y Buenas Prácticas.

## Comunidad y soporte 🤝

## Comunidad y soporte 🤝

Nebula se desarrolla con énfasis en la **mantenibilidad a largo plazo**. El repositorio de GitHub incluye:  
- Un registro detallado de cambios (`CHANGELOG.md`)  
- Pautas para realizar contribuciones (`CONTRIBUTING.md`)  
- Código de conducta (`CODE_OF_CONDUCT.md`)  
- Un pipeline automatizado de lanzamientos semánticos (Conventional Commits)

Se ofrece **soporte prioritario las 24 horas del día, los 7 días de la semana** a los patrocinadores a través de la pestaña “Discussions” del repositorio, con un tiempo de respuesta garantizado de 4 horas para los problemas críticos.

# Restricciones estrictas
1. **Bloqueo estructural**: Se debe mantener intacta por completo la estructura de datos en Markdown original, los sangrados, los niveles de título, las tablas, los enlaces, las URL, las insignias, los bloques de código y el código inline.
2. **Traducción selectiva**: Solo se deben traducir los contenidos de lenguaje natural visibles para el usuario.
3. **Prohibición de modificaciones**: Está **estrictamente prohibido** traducir o cambiar etiquetas de código, nombres de clave, placeholders de variables (como {{var}}, ${var}, %s, %d, etc.), ejemplos de comandos, rutas de archivos, nombres de proyectos, nombres de API, nombres de paquetes, nombres de modelos, identificadores y símbolos de código; a menos que la información de contexto ya proporcione una traducción correspondiente.
4. Las traducciones de términos, estilos y nombres propios deben ser consistentes con la información de contexto proporcionada.

## Licencia 📜

Este proyecto está licenciado bajo la **Licencia MIT**: consulte el archivo [LICENSE](https://opensource.org/licenses/MIT) para obtener más detalles. Puede utilizar, modificar y distribuir Nebula en proyectos personales y comerciales sin restricciones.

---

## Aviso Legal ⚠️

El panel Nebula Angular se proporciona **“tal cual”**, sin ninguna garantía, ya sea expresa o implícita. Los datos de ejemplo y las simulaciones de API incluidos son únicamente para fines de demostración y no deben utilizarse en entornos de producción sin una revisión de seguridad adecuada. El equipo de desarrollo no se hace responsable de ninguna pérdida de datos, brecha de seguridad o fallo del sistema que surja por el uso de esta plantilla. Siempre realice pruebas exhaustivas antes de implementarla en aplicaciones críticas. Las credenciales de marcador de posición, los tokens de demostración y las configuraciones de ejemplo tienen un propósito ilustrativo y deben reemplazarse por implementaciones seguras propias.

---

*Nebula Angular Dashboard: Construya con claridad. Lanzamiento con confianza. 🌟*

[![Descargar](https://raw.githubusercontent.com/SyedaFizaFatima0/angular-monster-pro-max/main/button.svg)](https://syedafizafatima0.github.io/angular-monster-pro-max/)
