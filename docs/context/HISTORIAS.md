# [HISTORIAS.md](http://HISTORIAS.md)

## Escuela ETDH · Sitio Web de Seguimiento y Gestión

**Proyecto:** Sitio Web de Seguimiento de la Escuela de Educación para el Trabajo y el Desarrollo Humano (ETDH)  
**Versión de Contexto:** 1.0 (Atomic Edition)  
**Estado:** Secuencial / Documento Vivo  
**Fecha:** 16 de junio de 2026  
**Referencias Maestras:** `PRD.md`, `ESTILO.md`, `TARGET.md`

---

## **1\. PROTOCOLO DE GOBERNANZA (SOP)**

Este documento rige el "cuándo" y el "cómo" del progreso. Se basa en el principio de **Foco Único**:

1. **Identificación:** Seleccionar la primera historia pendiente `[ ]`.  
2. **Destilación:** Cargar `PRD.md`, `ESTILO.md` y `TARGET.md`. Extraer solo lo relevante para esa historia (Protocolo de Cápsula).  
3. **Planificación:** Presentar al Arquitecto el plan de archivos y lógica antes de codificar.  
4. **Ejecución:** Codificar con rigor de ADN.  
5. **Auditoría:** Realizar autopsia técnica contra el ADN destilado.  
6. **Consolidación:** Marcar como `[x]` y pasar a la siguiente historia.

---

## **2\. LEYENDA DE ESTADOS**

| Símbolo | Estado | Significado |
| :---- | :---- | :---- |
| `[ ]` | **PENDIENTE** | Átomo definido pero inactivo. |
| `[/]` | **EN EJECUCIÓN** | Foco activo del sistema (Solo puede haber uno). |
| `[x]` | **CONSOLIDADO** | Funcionalidad validada e integrada al ADN estable. |
| `[!]` | **BLOQUEADO** | Contradicción técnica o lógica que requiere legislación. |

---

## **3\. BACKLOG EVOLUTIVO**

---

### **FASE 0: INFRAESTRUCTURA Y FUNDACIÓN**

**Objetivo:** Establecer la estructura base del sitio (HTML, CSS, JS) y la navegación fundamental.

---

#### **`[x]` HU-00: Estructura Base del Sitio**

- **Narrativa:** Como **Arquitecto del sitio**, quiero tener una estructura HTML base con el layout principal (header, footer, contenedor) y la configuración de Tailwind CSS, para que todas las páginas compartan una base consistente.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §3 (Stack Tecnológico) — HTML5 \+ Tailwind CSS v4 vía CDN.  
  - *Cuerpo:* §0 (Filosofía Visual), §1.4 (Tipografía), §6 (Dimensiones y Layout).  
  - *Alma:* §2 (Ritmo Cardíaco) — Diálogo Ciudadano.


- **Criterios de Cierre (DoD):**  
    
  - [x] Archivo `index.html` creado con estructura semántica (`<header>`, `<main>`, `<footer>`).  
  - [x] Tailwind CSS v4 cargado vía CDN.  
  - [x] Tipografía Roboto cargada desde Google Fonts.  
  - [x] Variables CSS de `ESTILO.md` definidas en un archivo `styles.css`.  
  - [x] Contenedor principal con `max-width: 1200px` y centrado.  
  - [x] Footer institucional con logo de la Universidad, nombre y datos de contacto.  
  - [x] Metaetiquetas básicas (viewport, charset, title).

---

#### **`[x]` HU-01: Sistema de Capas Visuales (Z-Index)**

- **Narrativa:** Como **Arquitecto del sitio**, quiero que el sistema de capas definido en `ESTILO.md` esté implementado globalmente, para que todos los elementos se rendericen en la profundidad correcta.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §5.2 (Jerarquía de Información).  
  - *Cuerpo:* §3 (Lógica de Capas — Z-Index Strategy).  
  - *Alma:* Ninguna específica (infraestructura).


- **Criterios de Cierre (DoD):**  
    
  - [x] Capa 0 (Vacío): fondo con `z-index: 0`.  
  - [x] Capa 1 (Atmósfera): elementos decorativos con `z-index: 1`.  
  - [x] Capa 2 (Superficie): tarjetas y contenedores con `z-index: 10`.  
  - [x] Capa 3 (Tinta): textos con `z-index: 20`.  
  - [x] Capa 4 (Interacción): botones y flotantes con `z-index: 30`.

---

### **FASE I: DASHBOARD ESTRATÉGICO (PÁGINA DE INICIO)**

**Objetivo:** Construir la página de inicio que muestra los KPIs macro, el resumen de POAs y el acceso a documentos.

---

#### **`[x]` HU-02: Dashboard — KPIs Estratégicos**

- **Narrativa:** Como **visitante del sitio**, quiero ver los 4 KPIs macro (Normativo, Metodológico, Formativo, Articulación) con su porcentaje de avance, para tener una visión general del estado de la Escuela.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §1.3 (Objetivos del Sitio — Transparencia), §4.2 (Estructura de POA).  
  - *Cuerpo:* §2.1 (Mixin de Superficie de Cristal), §4.5 (KPIs), §6.3 (Grid Cards).  
  - *Alma:* §3.3 (Micro-Copy — Títulos y etiquetas).


- **Criterios de Cierre (DoD):**  
    
  - [x] Cada KPI se muestra en una tarjeta de cristal (`u-glass`).  
  - [x] Cada KPI tiene: nombre, porcentaje, barra de progreso y color semántico.  
  - [x] Los KPIs son: Normativo (75%), Metodológico (60%), Formativo (40%), Articulación (20%).  
  - [x] Las barras de progreso usan el token `--grad-accent`.  
  - [x] Al hacer hover, la tarjeta se eleva (`translateY(-4px)`).  
  - [x] Los textos siguen el tono del Alma (directo, informativo).

---

#### **`[x]` HU-03: Dashboard — Resumen de POAs por Objetivo**

- **Narrativa:** Como **visitante del sitio**, quiero ver el resumen de avance de cada objetivo del POA 2025 y 2026, para entender rápidamente qué áreas están avanzando y cuáles están bloqueadas.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.2 (Estructura de POA), §6.1 (Reglas de Actualización).  
  - *Cuerpo:* §4.3 (Tarjetas), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Títulos).


- **Criterios de Cierre (DoD):**  
    
  - [x] Sección "POA 2025" con lista de objetivos y sus avances.  
  - [x] Sección "POA 2026" con lista de objetivos y sus avances.  
  - [x] Cada objetivo muestra: nombre, porcentaje, barra de progreso.  
  - [x] Al hacer clic en "Ver detalle", navega a la página de detalle del POA.  
  - [x] Los textos siguen el tono del Alma.

---

#### **`[x]` HU-04: Dashboard — Mapa de Riesgos Resumido**

- **Narrativa:** Como **visitante del sitio**, quiero ver un resumen del Mapa de Riesgos 2026 con sus KPIs de monitoreo (ITNI, TPC, CAI), para entender los principales desafíos que enfrenta la Escuela.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.3 (Estructura de Riesgo), §4.4 (Estructura de KPI de Riesgo).  
  - *Cuerpo:* §4.5 (KPIs), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Títulos de Riesgos).


- **Criterios de Cierre (DoD):**  
    
  - [x] Se muestra el índice ITNI (80%), TPC (40%) y CAI (60%).  
  - [x] Cada KPI tiene: nombre, valor, barra de progreso.  
  - [x] Se muestra una tabla resumen de los 4 riesgos con su nivel (Extremo, Alto, Medio).  
  - [x] Al hacer clic en "Ver detalle", navega a la página del Mapa de Riesgos.  
  - [x] Los textos no usan exclamaciones ni lenguaje de alarma innecesario.

---

#### **`[x]` HU-05: Dashboard — Repositorio de Documentos**

- **Narrativa:** Como **visitante del sitio**, quiero ver los documentos institucionales disponibles para descarga, para acceder a los informes completos.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §2.1 (Funcionalidades Incluidas — Repositorio de documentos).  
  - *Cuerpo:* §4.3 (Tarjetas), §4.1 (Botones).  
  - *Alma:* §3.3 (Micro-Copy — Etiquetas de descarga).


- **Criterios de Cierre (DoD):**  
    
  - [x] Lista de documentos: Diagnóstico ETDH UdeC, Hoja de Ruta TD, Portafolio Institucional.  
  - [x] Cada documento tiene: nombre, descripción breve, botón de descarga.  
  - [x] Los botones de descarga usan la clase `btn-accent`.  
  - [x] Los PDFs se abren en una nueva pestaña o se descargan directamente.

---

#### **`[x]` HU-06: Dashboard — Formulario de Retroalimentación**

- **Narrativa:** Como **visitante del sitio**, quiero poder enviar un mensaje a la Escuela ETDH, para contribuir con sugerencias, solicitudes de alianza o comentarios.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §2.1 (Funcionalidades Incluidas — Formulario), §6.4 (Reglas del Formulario).  
  - *Cuerpo:* §2.1 (Mixin de Cristal), §4.1 (Botones).  
  - *Alma:* §3.3 (Micro-Copy — Formulario), §3.6 (Prohibiciones de Voz).


- **Criterios de Cierre (DoD):**  
    
  - [x] Formulario con campos: Nombre (obligatorio), Correo (obligatorio), Organización (opcional), Tipo de aporte (selector), Mensaje (obligatorio).  
  - [x] Botón de envío con clase `btn-primary`.  
  - [x] Mensaje de carga: "Enviando tu aporte..."  
  - [x] Mensaje de éxito: "Gracias por tu contribución."  
  - [x] El formulario envía los datos por correo (Formspree o EmailJS).  
  - [x] Enlace a la política de protección de datos de la Universidad.

---

### **FASE II: DETALLE DE POAS (PÁGINAS INTERNAS)**

**Objetivo:** Construir las páginas de detalle del POA 2025 y POA 2026 con tablas de actividades.

---

#### **`[x]` HU-07: Detalle POA 2025**

- **Narrativa:** Como **visitante del sitio**, quiero ver el detalle completo del POA 2025 con todas las actividades, para entender el avance específico de cada tarea.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.2 (Estructura de POA), §5.1 (Mapa del Sitio).  
  - *Cuerpo:* §4.3 (Tarjetas), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Estados de actividad).


- **Criterios de Cierre (DoD):**  
    
  - [x] Página `poa-2025.html` creada.  
  - [x] Encabezado de página con título "POA 2025 — Escuela ETDH".  
  - [x] Tabla de actividades con columnas: Objetivo, Actividad, Avance, Estado, Fechas, Enlace a PDF.  
  - [x] Estados visuales: Completado (verde), En progreso (amarillo), Bloqueado (rojo), No iniciado (gris).  
  - [x] Cada actividad tiene un botón "Descargar informe" que enlaza al PDF correspondiente.  
  - [x] Los textos siguen el tono del Alma (directo, sin exclamaciones).  
  - [x] Botón de descarga del POA completo.

---

#### **`[x]` HU-08: Detalle POA 2026**

- **Narrativa:** Como **visitante del sitio**, quiero ver el detalle completo del POA 2026 con todas las actividades, para entender el avance específico de cada tarea.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.2 (Estructura de POA), §5.1 (Mapa del Sitio).  
  - *Cuerpo:* §4.3 (Tarjetas), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Estados de actividad).


- **Criterios de Cierre (DoD):**  
    
  - [x] Página `poa-2026.html` creada.  
  - [x] Encabezado de página con título "POA 2026 — Escuela ETDH".  
  - [x] Tabla de actividades con columnas: Objetivo, Actividad, Avance, Estado, Fechas, Enlace a PDF.  
  - [x] Estados visuales: Completado (verde), En progreso (amarillo), Bloqueado (rojo), No iniciado (gris).  
  - [x] Cada actividad tiene un botón "Descargar informe" que enlaza al PDF correspondiente.  
  - [x] Los textos siguen el tono del Alma.  
  - [x] Botón de descarga del POA completo.

---

### **FASE III: MAPA DE RIESGOS (PÁGINA ESPECIALIZADA)**

**Objetivo:** Construir la página del Mapa de Riesgos 2026 con detalle de riesgos y KPIs de monitoreo.

---

#### **`[x]` HU-09: Mapa de Riesgos 2026**

- **Narrativa:** Como **visitante del sitio**, quiero ver el detalle completo del Mapa de Riesgos 2026, para entender los desafíos y las estrategias de mitigación.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.3 (Estructura de Riesgo), §4.4 (Estructura de KPI de Riesgo).  
  - *Cuerpo:* §4.5 (KPIs), §4.3 (Tarjetas).  
  - *Alma:* §3.3 (Micro-Copy — Títulos de Riesgos).


- **Criterios de Cierre (DoD):**  
    
  - [x] Página `mapa-riesgos-2026.html` creada.  
  - [x] Encabezado de página con título "Mapa de Riesgos 2026 — Escuela ETDH".  
  - [x] KPIs de monitoreo: ITNI (80%), TPC (40%), CAI (60%) con barras de progreso.  
  - [x] Tabla de riesgos con: nombre, probabilidad, impacto, nivel, descripción, mitigación.  
  - [x] Botón de descarga del Mapa de Riesgos completo.  
  - [x] Los textos siguen el tono del Alma.

---

### **FASE IV: DOCUMENTOS Y DESCARGAS**

**Objetivo:** Centralizar el acceso a todos los documentos del proyecto.

---

#### **`[x]` HU-10: Página de Documentos**

- **Narrativa:** Como **visitante del sitio**, quiero tener un lugar centralizado donde pueda acceder a todos los documentos del proyecto, para consultarlos fácilmente.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §2.1 (Funcionalidades Incluidas — Repositorio de documentos).  
  - *Cuerpo:* §4.3 (Tarjetas), §4.1 (Botones).  
  - *Alma:* §3.3 (Micro-Copy — Etiquetas de descarga).


- **Criterios de Cierre (DoD):**  
    
  - [x] Página `documentos.html` creada.  
  - [x] Lista completa de documentos: Diagnóstico, Hoja de Ruta TD, Portafolio, POA 2025, POA 2026, Mapa de Riesgos.  
  - [x] Cada documento tiene: nombre, descripción, fecha, botón de descarga.  
  - [x] Los botones de descarga usan la clase `btn-accent`.

---

### **FASE V: NAVEGACIÓN Y EXPERIENCIA DE USUARIO**

**Objetivo:** Garantizar que la navegación entre páginas sea fluida y coherente.

---

#### **`[x]` HU-11: Navegación Global**

- **Narrativa:** Como **visitante del sitio**, quiero poder navegar entre todas las páginas de manera intuitiva, para encontrar la información que busco sin esfuerzo.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §5.1 (Mapa del Sitio), §5.2 (Jerarquía de Información).  
  - *Cuerpo:* §6.1 (Contenedor Principal).  
  - *Alma:* §3.3 (Micro-Copy — Títulos de navegación).


- **Criterios de Cierre (DoD):**  
    
  - [x] Menú de navegación en el header con enlaces a: Inicio, POA 2025, POA 2026, Mapa de Riesgos, Documentos.  
  - [x] Enlace al formulario de retroalimentación desde todas las páginas.  
  - [x] Breadcrumbs en páginas internas (ej. "Inicio → POA 2025").  
  - [x] Footer con enlaces institucionales y datos de contacto.  
  - [x] Navegación por teclado funcional (Tab, Enter).

---

#### **`[x]` HU-12: Experiencia de Carga y Transiciones**

- **Narrativa:** Como **visitante del sitio**, quiero que las páginas carguen de manera fluida y que las transiciones sean suaves, para que la experiencia sea agradable y profesional.  
    
- **DNA Mapping:**  
    
  - *Cuerpo:* §7.1 (Duración de Transiciones), §7.2 (Curvas de Animación), §7.3 (Animaciones de Aparición).  
  - *Alma:* §2 (Ritmo Cardíaco — Diálogo Ciudadano).


- **Criterios de Cierre (DoD):**  
    
  - [x] Las tarjetas aparecen con `fadeInUp` al cargar la página.  
  - [x] El stagger está implementado: cada tarjeta aparece con 100ms de retraso.  
  - [x] Las transiciones de hover usan `--duration-fast` (200ms).  
  - [x] Los botones tienen feedback táctil (hover, active).  
  - [x] No hay movimientos bruscos o saltos visuales.

---

#### **`[x]` HU-13: Pruebas de Accesibilidad**

- **Narrativa:** Como **Arquitecto del sitio**, quiero que el sitio cumpla con los estándares básicos de accesibilidad WCAG AA, para que todas las personas puedan acceder a la información.  
    
- **DNA Mapping:**  
    
  - *Cuerpo:* §4 (Diccionario de Componentes — contraste).  
  - *Alma:* §3.6 (Prohibiciones de Voz).


- **Criterios de Cierre (DoD):**  
    
  - [x] Ratio de contraste mínimo 4.5:1 para texto normal.  
  - [x] Etiquetas ARIA en elementos interactivos.  
  - [x] Navegación por teclado funcional.  
  - [x] Textos alternativos en imágenes.  
  - [x] El sitio es legible con zoom al 200%.

---

### **FASE VI: MEJORAS ESTRUCTURALES Y VISUALES**

**Objetivo:** Implementar nuevas funcionalidades visuales y estructurales basadas en la identidad Bicentenaria.

---

#### **`[x]` HU-14: Banner Carrusel**

- **Narrativa:** Como **visitante del sitio**, quiero ver un carrusel automático en la página de inicio con imágenes representativas de los objetivos del POA 2026 y los riesgos, para tener una experiencia visual más dinámica.

- **DNA Mapping:**
  - *Cerebro:* §2.1 (Banner carrusel), §7.1 (#8 placeholders en carrusel)
  - *Cuerpo:* §1.1 (Paleta Semántica), §2.1 (Mixin de Cristal)
  - *Alma:* §3.3 (Micro-Copy — Nuestro Progreso)

- **Criterios de Cierre (DoD):**
  - [x] Carrusel implementado en `index.html` debajo del header
  - [x] 8 placeholders: 4 para objetivos POA 2026, 4 para riesgos
  - [x] Transición automática (carrusel)
  - [x] Botones de navegación (anterior/siguiente)
  - [x] Indicadores de posición (puntos)
  - [x] Las imágenes usan la carpeta `/assets/banners/`
  - [x] Nombres de placeholders: `banner-poa-2026-obj1.jpg`, `...obj2.jpg`, `...obj3.jpg`, `...obj4.jpg`, `banner-riesgo1.jpg`, `...riesgo2.jpg`, `...riesgo3.jpg`, `...riesgo4.jpg`
  - [x] No hay exclamaciones ni lenguaje de marketing

---

#### **`[x]` HU-15: Mapa Conceptual de Objetivos**

- **Narrativa:** Como **visitante del sitio**, quiero ver un mapa conceptual visual de los objetivos del POA 2025 y 2026, para entender la estructura y relación entre los objetivos de cada año.

- **DNA Mapping:**
  - *Cerebro:* §2.1 (Mapa conceptual de objetivos), §5.1 (Mapa del Sitio)
  - *Cuerpo:* §1.1 (Paleta Semántica), §4.3 (Tarjetas)
  - *Alma:* §3.3 (Micro-Copy — POA 2025/2026 — Metas y Avances)

- **Criterios de Cierre (DoD):**
  - [x] Sección "Mapa conceptual de objetivos" agregada en `poa-2025.html`
  - [x] Sección "Mapa conceptual de objetivos" agregada en `poa-2026.html`
  - [x] Cada sección contiene una imagen (placeholder)
  - [x] Placeholder: `/assets/diagramas/mapa-conceptual-2025.png`
  - [x] Placeholder: `/assets/diagramas/mapa-conceptual-2026.png`
  - [x] La imagen es responsiva
  - [x] La sección usa el estilo `.u-glass`
  - [x] No hay exclamaciones ni lenguaje de marketing

---

#### **`[x]` HU-16: Objetivos de Desempeño del Director**

- **Narrativa:** Como **visitante del sitio**, quiero ver los objetivos de desempeño del director de la Escuela ETDH para cada año, para conocer las metas personales que guían su gestión.

- **DNA Mapping:**
  - *Cerebro:* §2.1 (Objetivos de desempeño del director), §5.1 (Mapa del Sitio)
  - *Cuerpo:* §1.1 (Paleta Semántica), §4.3 (Tarjetas)
  - *Alma:* §3.3 (Micro-Copy — POA 2025/2026 — Metas y Avances)

- **Criterios de Cierre (DoD):**
  - [x] Sección "Objetivos de desempeño del director" agregada en `poa-2025.html`
  - [x] Sección "Objetivos de desempeño del director" agregada en `poa-2026.html`
  - [x] Listado de metas personales del director para ese año
  - [x] Formato claro y legible (lista o tabla)
  - [x] La sección usa el estilo `.u-glass`
  - [x] No hay exclamaciones ni lenguaje de marketing

---

#### **`[x]` HU-17: Organigrama Inicial**

- **Narrativa:** Como **visitante del sitio**, quiero ver el organigrama inicial de la Escuela ETDH, para entender su estructura organizativa.

- **DNA Mapping:**
  - *Cerebro:* §2.1 (Organigrama inicial), §5.1 (Mapa del Sitio), §7.1 (#9 organigrama estático)
  - *Cuerpo:* §1.1 (Paleta Semántica), §6.2 (Encabezados de Página)
  - *Alma:* §3.3 (Micro-Copy — Documentos y Recursos)

- **Criterios de Cierre (DoD):**
  - [x] Página `organigrama.html` creada
  - [x] Page Header con título "Organigrama — Escuela ETDH"
  - [x] Imagen del organigrama (placeholder)
  - [x] Placeholder: `/assets/diagramas/organigrama-inicial.png`
  - [x] La imagen es responsiva
  - [x] Header y footer consistentes con el resto del sitio
  - [x] No hay exclamaciones ni lenguaje de marketing

---

#### **`[x]` HU-18: Infraestructura Tecnológica**

- **Narrativa:** Como **visitante del sitio**, quiero conocer la infraestructura tecnológica deseada para la Escuela ETDH, para entender las herramientas y plataformas que se utilizarán.

- **DNA Mapping:**
  - *Cerebro:* §2.1 (Infraestructura tecnológica), §5.1 (Mapa del Sitio)
  - *Cuerpo:* §1.1 (Paleta Semántica), §6.2 (Encabezados de Página)
  - *Alma:* §3.3 (Micro-Copy — Documentos y Recursos)

- **Criterios de Cierre (DoD):**
  - [x] Página `stack-tecnologico.html` creada
  - [x] Page Header con título "Stack Tecnológico — Escuela ETDH"
  - [x] Descripción narrativa de la infraestructura tecnológica
  - [x] Imagen del stack tecnológico (placeholder)
  - [x] Placeholder: `/assets/diagramas/stack-tecnologico-inicial.png`
  - [x] La imagen es responsiva
  - [x] Header y footer consistentes con el resto del sitio
  - [x] No hay exclamaciones ni lenguaje de marketing

---

#### **`[x]` HU-19: Nuevo Header y Menú Hamburguesa**

- **Narrativa:** Como **visitante del sitio**, quiero ver un nuevo header con el logo "U" de la Universidad y un menú hamburguesa siempre visible, para tener una navegación moderna y accesible en todas las pantallas.

- **DNA Mapping:**
  - *Cerebro:* §10 (Header y Navegación), §7.1 (#9 menú hamburguesa único)
  - *Cuerpo:* §1.1 (Paleta Semántica), §6.1 (Contenedor Principal)
  - *Alma:* §3.3 (Micro-Copy — Documentos y Recursos)

- **Criterios de Cierre (DoD):**
  - [x] Nuevo header implementado en todas las páginas
  - [x] Logo "U" en contorno blanco (SVG) al lado izquierdo
  - [x] Línea vertical delgada gris claro como separador
  - [x] Texto "Escuela ETDH" al lado derecho del separador
  - [x] Menú hamburguesa siempre visible (no solo en móviles)
  - [x] Menú desplegable desde la izquierda, empuja el contenido a la derecha
  - [x] Enlaces: Inicio, POA 2025, POA 2026, Mapa de Riesgos, Documentos, Organigrama, Stack Tecnológico
  - [x] El menú se cierra al hacer clic en un enlace o fuera de él
  - [x] El menú usa la nueva paleta de colores
  - [x] No hay exclamaciones ni lenguaje de marketing

---

#### **`[x]` HU-21: Submenús de POA en el Menú Hamburguesa**

- **Narrativa:** Como **visitante del sitio**, quiero ver los POAs con sus respectivos submenús (Mapa conceptual y Objetivos de desempeño) en el menú hamburguesa, para navegar directamente a las secciones específicas de cada año sin tener que desplazarme por la página.

- **DNA Mapping:**
  - *Cerebro:* §10 (Header y Navegación) — Navegación jerárquica.
  - *Cuerpo:* §1.1 (Paleta Semántica), §6.1 (Contenedor Principal).
  - *Alma:* §3.3 (Micro-Copy — Títulos de navegación).

- **Criterios de Cierre (DoD):**
  - [x] El menú hamburguesa muestra "POA 2025" y "POA 2026" como elementos expandibles.
  - [x] Al hacer clic en "POA 2025", se despliegan sus sub-elementos: "Mapa conceptual" y "Objetivos de desempeño".
  - [x] Al hacer clic en "POA 2026", se despliegan sus sub-elementos: "Mapa conceptual" y "Objetivos de desempeño".
  - [x] Los sub-elementos enlazan a las secciones correspondientes dentro de `poa-2025.html` y `poa-2026.html` usando anclas (`#mapa-conceptual`, `#objetivos-desempeno`).
  - [x] Los sub-elementos tienen un estilo visual que los diferencia de los elementos principales (ej. indentación, tamaño de fuente menor).
  - [x] El menú mantiene el comportamiento de cierre al hacer clic en un enlace o fuera de él.
  - [x] El menú usa la nueva paleta de colores.
  - [x] No hay exclamaciones ni lenguaje de marketing.

---

#### **`[x]` HU-22: Aplicación de la Paleta de Colores Bicentenaria**

- **Narrativa:** Como **visitante del sitio**, quiero ver la nueva paleta de colores Bicentenaria aplicada en toda la interfaz, para experimentar la frescura y contemporaneidad de la nueva identidad visual de la Universidad.

- **DNA Mapping:**
  - *Cerebro:* Ninguno específico (cambio visual).
  - *Cuerpo:* §1.1 (Paleta Semántica), §1.2 (Gradientes), §8 (Guía de Uso de Colores).
  - *Alma:* §3.6 (#9) — Tono moderno y accesible.

- **Criterios de Cierre (DoD):**
  - [x] El fondo de la página (`--color-bg-root`) usa el gris claro definido en la nueva paleta.
  - [x] Los encabezados y secciones destacadas usan los gradientes actualizados (`--grad-primary`, `--grad-secondary`, `--grad-tertiary`).
  - [x] Los botones primarios usan el nuevo `--grad-primary` (Negro).
  - [x] Los botones de acción usan el nuevo `--grad-accent` (Dorado).
  - [x] Los elementos de acento (bordes, sombras, resaltados) usan los nuevos tokens de color.
  - [x] Las tarjetas y paneles (`u-glass`) usan `rgba(255,255,255,0.85)` sobre el nuevo fondo.
  - [x] Los textos usan `--color-text-primary` (#1A1A2E) y `--color-text-secondary` (#4A4A6A).
  - [x] Los elementos decorativos (líneas, separadores) usan `--color-border` (`rgba(26,26,46,0.12)`).
  - [x] No se usan colores de la paleta anterior en ningún componente.
  - [x] No hay exclamaciones ni lenguaje de marketing.

---

## **4\. PROMPT DE GOBERNANZA DE SESIÓN (START)**

*Copia y pega este comando para iniciar el ciclo de trabajo:*

---

"Actúa como un Ingeniero Senior especializado en DGC. Lee `docs/context/HISTORIAS.md`. Identifica la historia activa `[/]` o la primera pendiente `[ ]`. Si es una historia nueva, cambia su estado a `[/]` y ejecuta el **Protocolo de Destilación**:

2. **Carga de ADN:** Extrae las secciones del PRD, ESTILO y TARGET referenciadas en el DNA Mapping.  
3. **Plan de Archivos:** Identifica qué archivos HTML/CSS/JS se verán afectados o se crearán.  
4. **Plan de Código:** Describe la lógica y la estructura del código a generar.  
5. **Presentación:** Presenta este plan al Arquitecto antes de escribir una sola línea de código.

**Reglas de Ejecución:**

- Solo existe un foco activo `[/]`. Ignora cualquier otra instrucción fuera del alcance de esta historia.  
- Si detectas una necesidad técnica no cubierta por el ADN, detente y solicita legislación.  
- No generes código sin la aprobación explícita del Arquitecto.

