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

#### **`[ ]` HU-00: Estructura Base del Sitio**

- **Narrativa:** Como **Arquitecto del sitio**, quiero tener una estructura HTML base con el layout principal (header, footer, contenedor) y la configuración de Tailwind CSS, para que todas las páginas compartan una base consistente.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §3 (Stack Tecnológico) — HTML5 \+ Tailwind CSS v4 vía CDN.  
  - *Cuerpo:* §0 (Filosofía Visual), §1.4 (Tipografía), §6 (Dimensiones y Layout).  
  - *Alma:* §2 (Ritmo Cardíaco) — Diálogo Ciudadano.


- **Criterios de Cierre (DoD):**  
    
  - [ ] Archivo `index.html` creado con estructura semántica (`<header>`, `<main>`, `<footer>`).  
  - [ ] Tailwind CSS v4 cargado vía CDN.  
  - [ ] Tipografía Roboto cargada desde Google Fonts.  
  - [ ] Variables CSS de `ESTILO.md` definidas en un archivo `styles.css`.  
  - [ ] Contenedor principal con `max-width: 1200px` y centrado.  
  - [ ] Footer institucional con logo de la Universidad, nombre y datos de contacto.  
  - [ ] Metaetiquetas básicas (viewport, charset, title).

---

#### **`[ ]` HU-01: Sistema de Capas Visuales (Z-Index)**

- **Narrativa:** Como **Arquitecto del sitio**, quiero que el sistema de capas definido en `ESTILO.md` esté implementado globalmente, para que todos los elementos se rendericen en la profundidad correcta.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §5.2 (Jerarquía de Información).  
  - *Cuerpo:* §3 (Lógica de Capas — Z-Index Strategy).  
  - *Alma:* Ninguna específica (infraestructura).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Capa 0 (Vacío): fondo con `z-index: 0`.  
  - [ ] Capa 1 (Atmósfera): elementos decorativos con `z-index: 1`.  
  - [ ] Capa 2 (Superficie): tarjetas y contenedores con `z-index: 10`.  
  - [ ] Capa 3 (Tinta): textos con `z-index: 20`.  
  - [ ] Capa 4 (Interacción): botones y flotantes con `z-index: 30`.

---

### **FASE I: DASHBOARD ESTRATÉGICO (PÁGINA DE INICIO)**

**Objetivo:** Construir la página de inicio que muestra los KPIs macro, el resumen de POAs y el acceso a documentos.

---

#### **`[ ]` HU-02: Dashboard — KPIs Estratégicos**

- **Narrativa:** Como **visitante del sitio**, quiero ver los 4 KPIs macro (Normativo, Metodológico, Formativo, Articulación) con su porcentaje de avance, para tener una visión general del estado de la Escuela.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §1.3 (Objetivos del Sitio — Transparencia), §4.2 (Estructura de POA).  
  - *Cuerpo:* §2.1 (Mixin de Superficie de Cristal), §4.5 (KPIs), §6.3 (Grid Cards).  
  - *Alma:* §3.3 (Micro-Copy — Títulos y etiquetas).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Cada KPI se muestra en una tarjeta de cristal (`u-glass`).  
  - [ ] Cada KPI tiene: nombre, porcentaje, barra de progreso y color semántico.  
  - [ ] Los KPIs son: Normativo (75%), Metodológico (60%), Formativo (40%), Articulación (20%).  
  - [ ] Las barras de progreso usan el token `--grad-accent`.  
  - [ ] Al hacer hover, la tarjeta se eleva (`translateY(-4px)`).  
  - [ ] Los textos siguen el tono del Alma (directo, informativo).

---

#### **`[ ]` HU-03: Dashboard — Resumen de POAs por Objetivo**

- **Narrativa:** Como **visitante del sitio**, quiero ver el resumen de avance de cada objetivo del POA 2025 y 2026, para entender rápidamente qué áreas están avanzando y cuáles están bloqueadas.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.2 (Estructura de POA), §6.1 (Reglas de Actualización).  
  - *Cuerpo:* §4.3 (Tarjetas), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Títulos).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Sección "POA 2025" con lista de objetivos y sus avances.  
  - [ ] Sección "POA 2026" con lista de objetivos y sus avances.  
  - [ ] Cada objetivo muestra: nombre, porcentaje, barra de progreso.  
  - [ ] Al hacer clic en "Ver detalle", navega a la página de detalle del POA.  
  - [ ] Los textos siguen el tono del Alma.

---

#### **`[ ]` HU-04: Dashboard — Mapa de Riesgos Resumido**

- **Narrativa:** Como **visitante del sitio**, quiero ver un resumen del Mapa de Riesgos 2026 con sus KPIs de monitoreo (ITNI, TPC, CAI), para entender los principales desafíos que enfrenta la Escuela.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.3 (Estructura de Riesgo), §4.4 (Estructura de KPI de Riesgo).  
  - *Cuerpo:* §4.5 (KPIs), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Títulos de Riesgos).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Se muestra el índice ITNI (80%), TPC (40%) y CAI (60%).  
  - [ ] Cada KPI tiene: nombre, valor, barra de progreso.  
  - [ ] Se muestra una tabla resumen de los 4 riesgos con su nivel (Extremo, Alto, Medio).  
  - [ ] Al hacer clic en "Ver detalle", navega a la página del Mapa de Riesgos.  
  - [ ] Los textos no usan exclamaciones ni lenguaje de alarma innecesario.

---

#### **`[ ]` HU-05: Dashboard — Repositorio de Documentos**

- **Narrativa:** Como **visitante del sitio**, quiero ver los documentos institucionales disponibles para descarga, para acceder a los informes completos.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §2.1 (Funcionalidades Incluidas — Repositorio de documentos).  
  - *Cuerpo:* §4.3 (Tarjetas), §4.1 (Botones).  
  - *Alma:* §3.3 (Micro-Copy — Etiquetas de descarga).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Lista de documentos: Diagnóstico ETDH UdeC, Hoja de Ruta TD, Portafolio Institucional.  
  - [ ] Cada documento tiene: nombre, descripción breve, botón de descarga.  
  - [ ] Los botones de descarga usan la clase `btn-accent`.  
  - [ ] Los PDFs se abren en una nueva pestaña o se descargan directamente.

---

#### **`[ ]` HU-06: Dashboard — Formulario de Retroalimentación**

- **Narrativa:** Como **visitante del sitio**, quiero poder enviar un mensaje a la Escuela ETDH, para contribuir con sugerencias, solicitudes de alianza o comentarios.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §2.1 (Funcionalidades Incluidas — Formulario), §6.4 (Reglas del Formulario).  
  - *Cuerpo:* §2.1 (Mixin de Cristal), §4.1 (Botones).  
  - *Alma:* §3.3 (Micro-Copy — Formulario), §3.6 (Prohibiciones de Voz).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Formulario con campos: Nombre (obligatorio), Correo (obligatorio), Organización (opcional), Tipo de aporte (selector), Mensaje (obligatorio).  
  - [ ] Botón de envío con clase `btn-primary`.  
  - [ ] Mensaje de carga: "Enviando tu aporte..."  
  - [ ] Mensaje de éxito: "Gracias por tu contribución."  
  - [ ] El formulario envía los datos por correo (Formspree o EmailJS).  
  - [ ] Enlace a la política de protección de datos de la Universidad.

---

### **FASE II: DETALLE DE POAS (PÁGINAS INTERNAS)**

**Objetivo:** Construir las páginas de detalle del POA 2025 y POA 2026 con tablas de actividades.

---

#### **`[ ]` HU-07: Detalle POA 2025**

- **Narrativa:** Como **visitante del sitio**, quiero ver el detalle completo del POA 2025 con todas las actividades, para entender el avance específico de cada tarea.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.2 (Estructura de POA), §5.1 (Mapa del Sitio).  
  - *Cuerpo:* §4.3 (Tarjetas), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Estados de actividad).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Página `poa-2025.html` creada.  
  - [ ] Encabezado de página con título "POA 2025 — Escuela ETDH".  
  - [ ] Tabla de actividades con columnas: Objetivo, Actividad, Avance, Estado, Fechas, Enlace a PDF.  
  - [ ] Estados visuales: Completado (verde), En progreso (amarillo), Bloqueado (rojo), No iniciado (gris).  
  - [ ] Cada actividad tiene un botón "Descargar informe" que enlaza al PDF correspondiente.  
  - [ ] Los textos siguen el tono del Alma (directo, sin exclamaciones).  
  - [ ] Botón de descarga del POA completo.

---

#### **`[ ]` HU-08: Detalle POA 2026**

- **Narrativa:** Como **visitante del sitio**, quiero ver el detalle completo del POA 2026 con todas las actividades, para entender el avance específico de cada tarea.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.2 (Estructura de POA), §5.1 (Mapa del Sitio).  
  - *Cuerpo:* §4.3 (Tarjetas), §2.1 (Mixin de Cristal).  
  - *Alma:* §3.3 (Micro-Copy — Estados de actividad).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Página `poa-2026.html` creada.  
  - [ ] Encabezado de página con título "POA 2026 — Escuela ETDH".  
  - [ ] Tabla de actividades con columnas: Objetivo, Actividad, Avance, Estado, Fechas, Enlace a PDF.  
  - [ ] Estados visuales: Completado (verde), En progreso (amarillo), Bloqueado (rojo), No iniciado (gris).  
  - [ ] Cada actividad tiene un botón "Descargar informe" que enlaza al PDF correspondiente.  
  - [ ] Los textos siguen el tono del Alma.  
  - [ ] Botón de descarga del POA completo.

---

### **FASE III: MAPA DE RIESGOS (PÁGINA ESPECIALIZADA)**

**Objetivo:** Construir la página del Mapa de Riesgos 2026 con detalle de riesgos y KPIs de monitoreo.

---

#### **`[ ]` HU-09: Mapa de Riesgos 2026**

- **Narrativa:** Como **visitante del sitio**, quiero ver el detalle completo del Mapa de Riesgos 2026, para entender los desafíos y las estrategias de mitigación.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §4.3 (Estructura de Riesgo), §4.4 (Estructura de KPI de Riesgo).  
  - *Cuerpo:* §4.5 (KPIs), §4.3 (Tarjetas).  
  - *Alma:* §3.3 (Micro-Copy — Títulos de Riesgos).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Página `mapa-riesgos-2026.html` creada.  
  - [ ] Encabezado de página con título "Mapa de Riesgos 2026 — Escuela ETDH".  
  - [ ] KPIs de monitoreo: ITNI (80%), TPC (40%), CAI (60%) con barras de progreso.  
  - [ ] Tabla de riesgos con: nombre, probabilidad, impacto, nivel, descripción, mitigación.  
  - [ ] Botón de descarga del Mapa de Riesgos completo.  
  - [ ] Los textos siguen el tono del Alma.

---

### **FASE IV: DOCUMENTOS Y DESCARGAS**

**Objetivo:** Centralizar el acceso a todos los documentos del proyecto.

---

#### **`[ ]` HU-10: Página de Documentos**

- **Narrativa:** Como **visitante del sitio**, quiero tener un lugar centralizado donde pueda acceder a todos los documentos del proyecto, para consultarlos fácilmente.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §2.1 (Funcionalidades Incluidas — Repositorio de documentos).  
  - *Cuerpo:* §4.3 (Tarjetas), §4.1 (Botones).  
  - *Alma:* §3.3 (Micro-Copy — Etiquetas de descarga).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Página `documentos.html` creada.  
  - [ ] Lista completa de documentos: Diagnóstico, Hoja de Ruta TD, Portafolio, POA 2025, POA 2026, Mapa de Riesgos.  
  - [ ] Cada documento tiene: nombre, descripción, fecha, botón de descarga.  
  - [ ] Los botones de descarga usan la clase `btn-accent`.

---

### **FASE V: NAVEGACIÓN Y EXPERIENCIA DE USUARIO**

**Objetivo:** Garantizar que la navegación entre páginas sea fluida y coherente.

---

#### **`[ ]` HU-11: Navegación Global**

- **Narrativa:** Como **visitante del sitio**, quiero poder navegar entre todas las páginas de manera intuitiva, para encontrar la información que busco sin esfuerzo.  
    
- **DNA Mapping:**  
    
  - *Cerebro:* §5.1 (Mapa del Sitio), §5.2 (Jerarquía de Información).  
  - *Cuerpo:* §6.1 (Contenedor Principal).  
  - *Alma:* §3.3 (Micro-Copy — Títulos de navegación).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Menú de navegación en el header con enlaces a: Inicio, POA 2025, POA 2026, Mapa de Riesgos, Documentos.  
  - [ ] Enlace al formulario de retroalimentación desde todas las páginas.  
  - [ ] Breadcrumbs en páginas internas (ej. "Inicio → POA 2025").  
  - [ ] Footer con enlaces institucionales y datos de contacto.  
  - [ ] Navegación por teclado funcional (Tab, Enter).

---

#### **`[ ]` HU-12: Experiencia de Carga y Transiciones**

- **Narrativa:** Como **visitante del sitio**, quiero que las páginas carguen de manera fluida y que las transiciones sean suaves, para que la experiencia sea agradable y profesional.  
    
- **DNA Mapping:**  
    
  - *Cuerpo:* §7.1 (Duración de Transiciones), §7.2 (Curvas de Animación), §7.3 (Animaciones de Aparición).  
  - *Alma:* §2 (Ritmo Cardíaco — Diálogo Ciudadano).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Las tarjetas aparecen con `fadeInUp` al cargar la página.  
  - [ ] El stagger está implementado: cada tarjeta aparece con 100ms de retraso.  
  - [ ] Las transiciones de hover usan `--duration-fast` (200ms).  
  - [ ] Los botones tienen feedback táctil (hover, active).  
  - [ ] No hay movimientos bruscos o saltos visuales.

---

#### **`[ ]` HU-13: Pruebas de Accesibilidad**

- **Narrativa:** Como **Arquitecto del sitio**, quiero que el sitio cumpla con los estándares básicos de accesibilidad WCAG AA, para que todas las personas puedan acceder a la información.  
    
- **DNA Mapping:**  
    
  - *Cuerpo:* §4 (Diccionario de Componentes — contraste).  
  - *Alma:* §3.6 (Prohibiciones de Voz).


- **Criterios de Cierre (DoD):**  
    
  - [ ] Ratio de contraste mínimo 4.5:1 para texto normal.  
  - [ ] Etiquetas ARIA en elementos interactivos.  
  - [ ] Navegación por teclado funcional.  
  - [ ] Textos alternativos en imágenes.  
  - [ ] El sitio es legible con zoom al 200%.

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

