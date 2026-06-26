# [ESTILO.md](http://ESTILO.md)

## Escuela ETDH · Sitio Web de Seguimiento y Gestión

**Proyecto:** Sitio Web de Seguimiento de la Escuela de Educación para el Trabajo y el Desarrollo Humano (ETDH)  
**Versión:** 1.0  
**Estado:** Inmutable / Referencia Absoluta  
**Fecha:** 16 de junio de 2026  
**Responsable:** Dirección de la Escuela ETDH — Vicerrectoría de Docencia, Universidad de Cartagena  
**Metodología:** Desarrollo Guiado por Contexto (DGC)

---

## **0\. Filosofía Visual (Identidad Bicentenaria)**

El sitio web de la Escuela ETDH es un **tablero de control institucional** que comunica honestidad, claridad y modernidad. Su identidad visual se fundamenta en la **paleta de colores Bicentenaria** de la Universidad de Cartagena, que aporta frescura, dinamismo y conecta con todos los públicos. La transparencia se mantiene como valor central, reflejada en el uso de cristal esmerilado y profundidad visual.

La metáfora física es: **un informe de gestión impreso en vidrio**. Los datos son claros, legibles, y el fondo institucional se mantiene presente pero no opaca la información.

**Se prohíben las superficies completamente planas.** Todo contenedor debe tener propiedades de material (vidrio, cristal esmerilado) que comuniquen transparencia y modernidad.

---

## **1\. La Constitución Atómica (Design Tokens)**

### **1.1. Paleta Semántica (Basada en el Manual Bicentenaria)**

| Token | Valor (Hex) | Uso Semántico |
| :---- | :---- | :---- |
| `--color-primary` | `#1A1A2E` | Negro institucional. Identidad, seriedad, tradición. |
| `--color-primary-dark` | `#0D0D1A` | Profundidad, énfasis. |
| `--color-accent` | `#F5A623` | Amarillo/Dorado. Luz, conocimiento, ciencia. |
| `--color-accent-light` | `#F7C948` | Brillo, juventud, energía. |
| `--color-accent-dark` | `#D4891A` | Sombra del dorado, madurez. |
| `--color-secondary` | `#6C2E8B` | Morado. Creatividad, visión, autenticidad. |
| `--color-secondary-light` | `#9B59B6` | Delicadeza, sensibilidad. |
| `--color-tertiary` | `#1ABC9C` | Turquesa. Equilibrio, calma, lealtad. |
| `--color-tertiary-light` | `#48C9B0` | Alegría, intuición. |
| `--color-cuaternary` | `#E67E22` | Naranja. Independencia, confianza, energía. |
| `--color-quinary` | `#2E86C1` | Azul. Libertad, armonía, seriedad. |
| `--color-text-primary` | `#1A1A2E` | Texto principal (casi negro). |
| `--color-text-secondary` | `#4A4A6A` | Texto secundario, metadatos. |
| `--color-text-inverse` | `#FFFFFF` | Texto sobre fondos oscuros. |
| `--color-bg-root` | `#F5F6FA` | Fondo general (gris muy claro). |
| `--color-surface` | `rgba(255, 255, 255, 0.85)` | Tarjetas y paneles (cristal). |
| `--color-border` | `rgba(26, 26, 46, 0.12)` | Bordes sutiles. |
| `--color-shadow` | `rgba(26, 26, 46, 0.08)` | Sombras coloreadas (no negras). |
| `--color-status-completed` | `#1ABC9C` | Estado de actividad "Completada". |
| `--color-status-progress` | `#F5A623` | Estado de actividad "En progreso". |
| `--color-status-blocked` | `#C0392B` | Estado de actividad "Bloqueada". |
| `--color-status-pending` | `#B0B0C0` | Estado de actividad "No iniciada". |
| `--color-risk-extreme` | `#C0392B` | Nivel de riesgo "Extremo". |
| `--color-risk-high` | `#E67E22` | Nivel de riesgo "Alto". |

### **1.2. Gradientes Semánticos**

| Token | Valor | Uso |
| :---- | :---- | :---- |
| `--grad-primary` | `linear-gradient(135deg, #1A1A2A, #0D0D1A)` | Fondos de encabezados, secciones destacadas. |
| `--grad-accent` | `linear-gradient(135deg, #F5A623, #D4891A)` | Botones de acción (dorado). |
| `--grad-secondary` | `linear-gradient(135deg, #6C2E8B, #9B59B6)` | Secciones creativas o de innovación. |
| `--grad-tertiary` | `linear-gradient(135deg, #1ABC9C, #48C9B0)` | Secciones de calma o equilibrio. |

### **1.3. Escala Espacial (Grid de 8px)**

| Token | Valor | Uso |
| :---- | :---- | :---- |
| `--space-xs` | `4px` | Micro-ajustes, iconos. |
| `--space-sm` | `8px` | Separación interna de botones. |
| `--space-md` | `16px` | Padding estándar de tarjetas. |
| `--space-lg` | `24px` | Separación entre secciones. |
| `--space-xl` | `48px` | Separación de bloques mayores. |
| `--space-2xl` | `80px` | Separación de páginas y secciones principales. |

**Regla:** Todo margen, padding y tamaño debe ser múltiplo de 4px. Valores como 13px o 21px son errores de compilación visual.

### **1.4. Tipografía (Extraída del Manual de Uso Web)**

| Elemento | Fuente | Uso |
| :---- | :---- | :---- |
| **Títulos (H1-H3)** | `Roboto` (Bold) | Encabezados, títulos de página. |
| **Cuerpo de texto** | `Roboto` (Regular) | Párrafos, descripciones. |
| **Datos / KPIs** | `Roboto` (Bold) | Números, indicadores (destacar). |
| **Metadatos** | `Roboto` (Light) | Fechas, responsables, etiquetas. |

**Regla de Implementación:**

font-family: 'Roboto', sans-serif;

**Escala Tipográfica:** | Token | Tamaño | Uso | |-------|--------|-----| | `--text-xs` | `0.75rem` (12px) | Metadatos, etiquetas. | | `--text-sm` | `0.875rem` (14px) | Texto secundario. | | `--text-base` | `1rem` (16px) | Texto principal. | | `--text-lg` | `1.25rem` (20px) | Subtítulos. | | `--text-xl` | `1.5rem` (24px) | Títulos H3. | | `--text-2xl` | `2rem` (32px) | Títulos H2. | | `--text-3xl` | `2.5rem` (40px) | Títulos H1. | | `--text-4xl` | `3rem` (48px) | Títulos de página. |

---

## **2\. El Motor de Física (Mixins y Clases Maestras)**

### **2.1. Mixin de Superficie de Cristal (Glassmorphism Técnico)**

Para todos los paneles, tarjetas y contenedores de contenido:

.u-glass {

  /\* Base: casi transparente \*/

  background: rgba(255, 255, 255, 0.72);

  

  /\* Física de la lente: difuminado y saturación \*/

  backdrop-filter: blur(20px) saturate(180%);

  \-webkit-backdrop-filter: blur(20px) saturate(180%);

  

  /\* Borde de luz: corte del cristal \*/

  border: 1px solid rgba(255, 255, 255, 0.25);

  

  /\* Sombra ambiental (coloreada, no negra) \*/

  box-shadow: 

    0 8px 32px rgba(0, 51, 160, 0.08),

    inset 0 1px 0 rgba(255, 255, 255, 0.3);

  

  /\* Esquinas suaves pero definidas \*/

  border-radius: 12px;

  

  /\* Transición suave para hover \*/

  transition: all var(--duration-medium, 300ms) cubic-bezier(0.25, 1, 0.5, 1);

}

.u-glass:hover {

  background: rgba(255, 255, 255, 0.85);

  box-shadow: 

    0 12px 48px rgba(0, 51, 160, 0.12),

    inset 0 1px 0 rgba(255, 255, 255, 0.4);

  transform: translateY(-2px);

}

### **2.2. Mixin de Superficie de Cristal Premium (Para elementos destacados)**

.u-glass-premium {

  background: rgba(255, 255, 255, 0.60);

  backdrop-filter: blur(25px) saturate(180%);

  \-webkit-backdrop-filter: blur(25px) saturate(180%);

  border: 1px solid rgba(255, 255, 255, 0.30);

  box-shadow: 

    0 8px 32px rgba(0, 51, 160, 0.06),

    inset 0 1px 0 rgba(255, 255, 255, 0.4);

  border-radius: 16px;

}

### **2.3. Mixin de Atmósfera (Textura de Fondo)**

Para el fondo de la página, se aplica un gradiente sutil con el patrón institucional:

.u-atmosphere {

  position: fixed;

  top: 0;

  left: 0;

  width: 100vw;

  height: 100vh;

  z-index: 0;

  background: 

    radial-gradient(ellipse at 10% 20%, rgba(0, 51, 160, 0.03) 0%, transparent 60%),

    radial-gradient(ellipse at 90% 80%, rgba(252, 227, 0, 0.03) 0%, transparent 60%),

    \#F5F7FA;

  pointer-events: none;

}

### **2.4. Mixin de Sombra Coloreada**

Para botones y elementos interactivos:

.u-shadow-glow {

  box-shadow: 

    0 8px 24px rgba(252, 227, 0, 0.30),

    0 2px 8px rgba(252, 227, 0, 0.15);

}

.u-shadow-blue {

  box-shadow: 

    0 8px 24px rgba(0, 51, 160, 0.20),

    0 2px 8px rgba(0, 51, 160, 0.10);

}

---

## **3\. Lógica de Capas (Z-Index Strategy)**

El sitio se construye como un **sándwich de materiales**, de abajo hacia arriba:

| Capa | Nombre | Contenido | Z-Index |
| :---- | :---- | :---- | :---- |
| **Capa 0** | El Vacío (Void) | Fondo de la página (gradientes y textura) | `0` |
| **Capa 1** | La Atmósfera (Atmosphere) | Elementos decorativos de fondo (patrón, orbes de luz) | `1` |
| **Capa 2** | La Superficie (Surface) | Tarjetas, paneles, contenedores de contenido | `10` |
| **Capa 3** | La Tinta (Ink) | Texto, iconos, datos, KPIs | `20` |
| **Capa 4** | La Interacción (Float) | Botones, enlaces, elementos flotantes, modales | `30` |

**Regla de Implementación:**

- Todo contenedor de contenido (Capa 2\) debe usar `position: relative` y `z-index: 10`.  
- Todo elemento interactivo (Capa 4\) debe usar `position: relative` y `z-index: 30`.  
- **Prohibido** colocar texto (Capa 3\) directamente sobre el Vacío (Capa 0\) sin un contenedor intermedio.

---

## **4\. Diccionario de Componentes (ADN Específico)**

### **4.1. Botones de Acción**

.btn-primary {

  display: inline-block;

  padding: var(--space-sm) var(--space-lg);

  background: var(--grad-primary);

  color: white;

  font-family: 'Roboto', sans-serif;

  font-weight: 700;

  font-size: var(--text-sm);

  text-transform: uppercase;

  letter-spacing: 0.05em;

  border: none;

  border-radius: 8px;

  cursor: pointer;

  transition: all 200ms cubic-bezier(0.05, 0.7, 0.1, 1);

  box-shadow: 0 4px 12px rgba(0, 51, 160, 0.25);

}

.btn-primary:hover {

  transform: translateY(-2px);

  box-shadow: 0 8px 24px rgba(0, 51, 160, 0.35);

}

.btn-primary:active {

  transform: translateY(0px);

  box-shadow: 0 2px 8px rgba(0, 51, 160, 0.20);

}

### **4.2. Botones de Acción Secundaria (Amarillo)**

.btn-accent {

  display: inline-block;

  padding: var(--space-sm) var(--space-lg);

  background: var(--grad-accent);

  color: var(--color-primary);

  font-family: 'Roboto', sans-serif;

  font-weight: 700;

  font-size: var(--text-sm);

  text-transform: uppercase;

  letter-spacing: 0.05em;

  border: none;

  border-radius: 8px;

  cursor: pointer;

  transition: all 200ms cubic-bezier(0.05, 0.7, 0.1, 1);

  box-shadow: 0 4px 12px rgba(252, 227, 0, 0.30);

}

.btn-accent:hover {

  transform: translateY(-2px);

  box-shadow: 0 8px 24px rgba(252, 227, 0, 0.45);

}

### **4.3. Tarjetas (Cards)**

.card {

  @apply u-glass;

  padding: var(--space-lg);

  margin-bottom: var(--space-md);

  transition: all 300ms cubic-bezier(0.25, 1, 0.5, 1);

}

.card:hover {

  transform: translateY(-4px);

  box-shadow: 0 12px 48px rgba(0, 51, 160, 0.10);

}

### **4.4. Encabezados de Sección**

.section-header {

  font-family: 'Roboto', sans-serif;

  font-weight: 700;

  font-size: var(--text-2xl);

  color: var(--color-primary);

  margin-bottom: var(--space-lg);

  padding-bottom: var(--space-sm);

  border-bottom: 3px solid var(--color-accent);

  display: inline-block;

}

### **4.5. KPIs (Indicadores Visuales)**

.kpi-container {

  display: inline-block;

  padding: var(--space-sm) var(--space-md);

  background: var(--color-primary);

  color: white;

  border-radius: 8px;

  font-weight: 700;

  font-family: 'Roboto', sans-serif;

}

.kpi-bar {

  height: 8px;

  background: rgba(255, 255, 255, 0.20);

  border-radius: 4px;

  overflow: hidden;

}

.kpi-bar-fill {

  height: 100%;

  background: var(--grad-accent);

  border-radius: 4px;

  transition: width 600ms cubic-bezier(0.25, 1, 0.5, 1);

}

---

## **5\. Anti-Patrones Visuales (El Sistema Inmunológico)**

| \# | Prohibición | Razón |
| :---- | :---- | :---- |
| 1 | ❌ **Superficies completamente planas** | Prohibido `background: #FFFFFF` o `background: #F5F7FA` sin `backdrop-filter` o textura. |
| 2 | ❌ **Sombras negras** | Prohibido `box-shadow: 0 5px 10px #000`. Usar `rgba(0, 51, 160, X.XX)`. |
| 3 | ❌ **Bordes grises o negros** | Prohibido `border: 1px solid #ccc`. Usar `rgba(255,255,255,0.15)` o `rgba(0,51,160,0.10)`. |
| 4 | ❌ **Radios de borde inconsistentes** | Usar un radio unificado: `8px` para elementos pequeños, `12px` para tarjetas, `16px` para paneles. |
| 5 | ❌ **Texto sin contraste suficiente** | Ratio mínimo 4.5:1 para texto normal (WCAG AA). |
| 6 | ❌ **Decoración sin propósito** | No hay ilustraciones, iconos decorativos o animaciones sin función informativa. |
| 7 | ❌ **Tipografías fuera de Roboto** | No se usan fuentes diferentes a `Roboto` para ningún texto. |
| 8 | ❌ **Imágenes de stock** | Las únicas imágenes permitidas son las institucionales (Escudo, logos) y los iconos de facultades del Manual. |
| 9 | ❌ **Exceso de colores** | Solo se usan los tokens definidos en la paleta semántica. |
| 10 | ❌ **Movimiento brusco** | Las transiciones deben ser suaves (`ease-out`, `cubic-bezier(0.25, 1, 0.5, 1)`). |
| 11 | ❌ **Uso excesivo de colores de la paleta Bicentenaria en una sola vista** | No saturar. Máximo 3 colores por sección. |
| 12 | ❌ **Amarillo/Dorado como color de fondo principal** | Su uso es para detalles y acentos, no para fondos extensos. |
| 13 | ❌ **Morado o Turquesa como colores primarios de texto** | Solo usar para títulos o elementos decorativos, no para texto corrido. |
| 14 | ❌ **Usar colores de estados o riesgos que no estén en la paleta definida** | Todos los estados y niveles de riesgo deben usar los tokens definidos en §10. |

---

## **6\. Dimensiones y Layout (Extraído del Manual de Uso Web)**

### **6.1. Contenedor Principal**

.container {

  max-width: 1200px;

  margin: 0 auto;

  padding: 0 var(--space-lg);

}

**Regla:** Todo el contenido informativo (textos, botones, KPIs) debe estar dentro de los 1200px centrales.

### **6.2. Encabezados de Página**

.page-header {

  background: var(--grad-primary);

  color: white;

  padding: var(--space-xl) 0;

  border-bottom: 4px solid var(--color-accent);

}

.page-header h1 {

  font-size: var(--text-4xl);

  font-weight: 700;

  margin-bottom: var(--space-sm);

}

.page-header p {

  font-size: var(--text-lg);

  opacity: 0.85;

}

### **6.3. Tarjetas en Grid**

.grid-cards {

  display: grid;

  grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));

  gap: var(--space-lg);

}

---

## **7\. Animaciones y Transiciones (Atmósfera de Transparencia)**

### **7.1. Duración de Transiciones**

| Token | Valor | Uso |
| :---- | :---- | :---- |
| `--duration-instant` | `80ms` | Hover de botones, feedback táctil. |
| `--duration-fast` | `200ms` | Cambios de estado, toggles. |
| `--duration-medium` | `350ms` | Apertura de paneles, scroll suave. |
| `--duration-slow` | `600ms` | Carga de elementos, aparición de secciones. |

### **7.2. Curvas de Animación**

| Token | Valor | Sensación |
| :---- | :---- | :---- |
| `--ease-tactile` | `cubic-bezier(0.05, 0.7, 0.1, 1)` | Respuesta rápida, frenado seco. Para botones. |
| `--ease-glass` | `cubic-bezier(0.25, 1, 0.5, 1)` | Suave, como vidrio flotando. Para tarjetas. |
| `--ease-organic` | `cubic-bezier(0.4, 0, 0.2, 1)` | Muy suave, para apariciones. |

### **7.3. Animaciones de Aparición**

@keyframes fadeInUp {

  from {

    opacity: 0;

    transform: translateY(20px);

  }

  to {

    opacity: 1;

    transform: translateY(0);

  }

}

.u-fade-in {

  animation: fadeInUp var(--duration-slow) var(--ease-glass) forwards;

}

---

## **8\. Guía de Uso de Colores (Bicentenaria)**

### **8.1. Colores Primarios (Identidad)**

- **Negro (`--color-primary`):** Usar en encabezados, títulos, elementos de alta jerarquía.
- **Amarillo/Dorado (`--color-accent`):** Usar en botones de acción, elementos de atención, resaltados.

### **8.2. Colores Secundarios (Énfasis y Frescura)**

- **Morado (`--color-secondary`):** Usar en secciones de innovación, creatividad o visión.
- **Turquesa (`--color-tertiary`):** Usar en secciones de equilibrio, calma o confianza.
- **Naranja (`--color-cuaternary`):** Usar en secciones de energía, independencia.
- **Azul (`--color-quinary`):** Usar en secciones de seriedad, verdad, armonía.

### **8.3. Reglas de Aplicación**

- **No usar más de 3 colores distintos en una misma sección.** La paleta ampliada es para variedad entre secciones, no para saturación.
- **El color de fondo general (`--color-bg-root`) debe mantenerse neutro (gris claro).**
- **Los colores de acento deben usarse con moderación para no perder su impacto.**

---

## **9\. Colores de Estados y Riesgos**

### **9.1. Estados de Actividades**

| Estado | Color de fondo | Color de texto | Token |
| :---- | :---- | :---- | :---- |
| Completada | `#1ABC9C` (Turquesa) | `#FFFFFF` | `--color-status-completed` |
| En progreso | `#F5A623` (Dorado) | `#1A1A2A` | `--color-status-progress` |
| Bloqueada | `#C0392B` (Rojo) | `#FFFFFF` | `--color-status-blocked` |
| No iniciada | `#B0B0C0` (Gris) | `#FFFFFF` | `--color-status-pending` |

### **9.2. Niveles de Riesgo**

| Nivel | Color de fondo | Color de texto | Token |
| :---- | :---- | :---- | :---- |
| Extremo | `#C0392B` (Rojo) | `#FFFFFF` | `--color-risk-extreme` |
| Alto | `#E67E22` (Naranja) | `#FFFFFF` | `--color-risk-high` |

### **9.3. Iconos de Riesgo**

| Nivel | Color del icono | Token |
| :---- | :---- | :---- |
| Extremo | `#C0392B` | `--color-risk-extreme` |
| Alto | `#E67E22` | `--color-risk-high` |

---

## **10\. Prompt de Gobernanza Visual**

**Este documento actúa como la Fuente Única de Verdad (Single Source of Truth) para la capa visual del sitio web de la Escuela ETDH.**

Cualquier clase CSS que generes debe derivar de estos tokens. Si el diseño requiere un color o medida nueva, no lo inventes (hardcode); declara un nuevo token semántico primero en este documento.

**Prioridades:**

1. **Transparencia**: Usar `backdrop-filter` y `rgba` para crear atmósfera de cristal.  
2. **Institucionalidad**: Respetar colores, tipografías y dimensiones del Manual de Uso Web.  
3. **Legibilidad**: Asegurar contraste WCAG AA (4.5:1 mínimo).  
4. **Consistencia**: Todos los componentes deben compartir la misma lógica de capas y materiales.

**Prohibido:**

- Usar colores que no estén en la paleta semántica.  
- Usar sombras negras o bordes grises.  
- Crear superficies planas sin `backdrop-filter` o textura.  
- Usar fuentes diferentes a `Roboto`.

Procede con rigor absoluto.

