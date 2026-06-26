# INFORME DE CIERRE — ESCUELA ETDH · SITIO WEB DE SEGUIMIENTO Y GESTIÓN

**Fecha:** 25 de Junio de 2026
**Versión:** 1.0 (Entrega Inicial)
**Responsable:** Director de la Escuela ETDH

---

## 1. Resumen Ejecutivo

El sitio web de la Escuela de Educación para el Trabajo y el Desarrollo Humano (ETDH) ha sido desarrollado en su totalidad, cumpliendo con los objetivos de transparencia, rendición de cuentas, comunicación de riesgos y participación ciudadana.

### 1.1. Entregables
- 8 páginas HTML completas y funcionales.
- Sistema de diseño coherente con el Manual de Identidad Visual Bicentenaria.
- Documentación completa del ADN del proyecto (PRD, ESTILO, TARGET, HISTORIAS).
- Contenido actualizado de POA 2025, POA 2026 y Mapa de Riesgos 2026.

### 1.2. Estado Actual
- **Funcionalidad:** 95% completada.
- **Pendiente:** Configuración de envío real de correos (Netlify Forms).

---

## 2. Estructura del Sitio

### 2.1. Páginas

| Página | Archivo | Estado | Descripción |
|--------|---------|--------|-------------|
| Dashboard | `index.html` | ✅ | Página principal con KPIs, resúmenes de POAs y Mapa de Riesgos |
| POA 2025 | `poa-2025.html` | ✅ | Detalle de actividades del Objetivo 1, 2 y 3 |
| POA 2026 | `poa-2026.html` | ✅ | Detalle de actividades del Objetivo 1, 2, 3 y 4 |
| Mapa de Riesgos | `mapa-riesgos-2026.html` | ✅ | Detalle de riesgos y KPIs de monitoreo |
| Organigrama | `organigrama.html` | ✅ | Organigrama inicial de la Escuela |
| Stack Tecnológico | `stack-tecnologico.html` | ✅ | Infraestructura tecnológica inicial |
| Diseño Curricular | `diseno-curricular-adaptaton.html` | ✅ | Documento principal + 8 anexos |
| Director ETDH | `director-etdh.html` | ✅ | 21 funciones con roles asumidos |

### 2.2. Navegación
- Menú hamburguesa en todas las páginas
- Breadcrumbs en páginas internas
- Submenús para POA 2025 y POA 2026 (Mapa conceptual, Objetivos de desempeño)
- Enlace "Director ETDH" al final del menú, separado por línea horizontal

---

## 3. Sistema de Diseño

| Elemento | Especificación | Estado |
|----------|----------------|--------|
| Header | [☰] Seguimiento y Gestión · [Logo] Escuela ETDH | ✅ |
| Footer | Recuadro "E" naranja (#E67E22) con enlace a la Universidad | ✅ |
| Paleta | Bicentenaria (#1A1A2A, #F5A623, #00A3C4, #6C2E8B, #1ABC9C, #E67E22) | ✅ |
| Glassmorphism | `.u-glass` con `backdrop-filter: blur(20px)` | ✅ |
| Barras de progreso | `--color-secondary` (Morado #6C2E8B) | ✅ |
| Subrayados de títulos | `--color-accent` (Dorado #F5A623) | ✅ |
| Iconos | Turquesa #00A3C4 en todas las clases `.icon-*` | ✅ |
| Niveles de riesgo | Extremo: Rojo (#C0392B), Alto: Naranja (#E67E22) | ✅ |
| Estados de actividad | Completada: Turquesa, En progreso: Dorado, Bloqueada: Rojo, No iniciada: Gris | ✅ |

---

## 4. Contenido Validado

### 4.1. POA 2025

| Objetivo | Avance | Estado |
|----------|--------|--------|
| Objetivo 1: Modelo Operativo y Ecosistema Tecnológico | 0% | ✅ |
| Objetivo 2: Modelo Metodológico y Adaptatón | 87% | ✅ |
| Objetivo 3: Alianzas Estratégicas y Propuesta de Valor | 76% | ✅ |

15 actividades con estados, tipos, fechas y enlaces a informes.

### 4.2. POA 2026

| Objetivo | Avance | Estado |
|----------|--------|--------|
| Objetivo 1: Formalización Jurídica y Administrativa | 54% | ✅ |
| Objetivo 2: Ejecución Adaptatón | 40% | ✅ |
| Objetivo 3: Nuevos Programas | 32% | ✅ |
| Objetivo 4: Ecosistema de Alianzas | 70% | ✅ |

15 actividades con estados, tipos, fechas y enlaces a informes.

### 4.3. Mapa de Riesgos 2026

| KPI | Valor | Descarga |
|-----|-------|----------|
| ITNI (Índice de Tracción Normativa Interna) | 80% | ✅ |
| TPC (Tasa de Prototipado Colaborativo) | 40% | ✅ |
| CAI (Coeficiente de Actualización "IA-Ready") | 60% | ✅ |

| Riesgo | Nivel | Probabilidad | Impacto |
|--------|-------|--------------|---------|
| Parálisis por Vacío Normativo Interno | Extremo | Muy Alta | Crítico |
| Obsolescencia IA en Oferta Académica | Alto | Media | Alto |
| Interrupción por Dependencia Unipersonal | Extremo | Alta | Crítico |
| Falla en Producción de Activos RED | Alto | Muy Alta | Alto |

Sección adicional: Mapa de Riesgos 2025 con botón de descarga.

### 4.4. Director ETDH
- 21 funciones completas
- Cada función con narrativa profesional y rol asumido
- Sin etiquetas de "Evidencia"

### 4.5. Diseño Curricular Adaptatón
- Documento principal (17 páginas)
- 8 anexos en 3 fases (Fase I: Anexos 1-4, Fase II: perfil de egreso, Fase III: Anexos 5-8)

---

## 5. Documentación del ADN

| Archivo | Estado | Contenido |
|---------|--------|-----------|
| `docs/context/PRD.md` | ✅ | Visión, alcance, restricciones, modelo de datos, header/navegación |
| `docs/context/ESTILO.md` | ✅ | Paleta Bicentenaria, 22 tokens, gradientes, estados y riesgos |
| `docs/context/TARGET.md` | ✅ | Arquetipo Maestro de Obras, micro-copy, prohibiciones de voz |
| `docs/context/HISTORIAS.md` | ✅ | 21 HUs (00-22), todas consolidadas en Fase 0 a VI |
| `docs/context/REFERENCIA_FUNCIONES.md` | ✅ | Lista maestra de 21 funciones del Director |
| `README.md` | ✅ | Documentación del proyecto, instalación y uso |
| `AGENTS.md` | ✅ | Configuración de reglas para OpenCode |

---

## 6. Historial de Usuarios

| HU | Nombre | Estado |
|----|--------|--------|
| HU-00 | Estructura Base del Sitio | ✅ |
| HU-01 | Sistema de Capas Visuales (Z-Index) | ✅ |
| HU-02 | Dashboard — KPIs Estratégicos | ✅ |
| HU-03 | Dashboard — Resumen de POAs por Objetivo | ✅ |
| HU-04 | Dashboard — Mapa de Riesgos Resumido | ✅ |
| HU-05 | Dashboard — Repositorio de Documentos | ✅ |
| HU-06 | Dashboard — Formulario de Retroalimentación | ✅ |
| HU-07 | Detalle POA 2025 | ✅ |
| HU-08 | Detalle POA 2026 | ✅ |
| HU-09 | Mapa de Riesgos 2026 | ✅ |
| HU-10 | Página de Documentos | ✅ |
| HU-11 | Navegación Global | ✅ |
| HU-12 | Experiencia de Carga y Transiciones | ✅ |
| HU-13 | Pruebas de Accesibilidad | ✅ |
| HU-14 | Banner Carrusel | ✅ |
| HU-15 | Mapa Conceptual de Objetivos | ✅ |
| HU-16 | Objetivos de Desempeño del Director | ✅ |
| HU-17 | Organigrama Inicial | ✅ |
| HU-18 | Infraestructura Tecnológica | ✅ |
| HU-19 | Nuevo Header y Menú Hamburguesa | ✅ |
| HU-21 | Submenús de POA en el Menú Hamburguesa | ✅ |
| HU-22 | Aplicación de la Paleta de Colores Bicentenaria | ✅ |

---

## 7. Sección "Documentos Institucionales" (index.html)

| # | Documento | Archivo | Ruta |
|---|-----------|---------|------|
| 1 | Diagnóstico ETDH en Colombia (2015-2025) | `diagnostico-ETDH.pdf` | `documentos/informes/diagnostico-ETDH.pdf` |
| 2 | Hoja de Ruta para la Transformación Digital | `hoja-ruta-TD.pdf` | `documentos/informes/hoja-ruta-TD.pdf` |
| 3 | Manual de Operaciones y Procedimientos (MOP) | `MOP_borrador.pdf` | `documentos/informes/MOP_borrador.pdf` |
| 4 | Diseño Curricular — Proyecto Adaptatón | `diseno-adaptaton.pdf` | `documentos/informes/diseno-adaptaton.pdf` |

---

## 8. Footer (Estructura Final)

- **Lado izquierdo:** Logo "E" naranja + "Escuela ETDH" + "Universidad de Cartagena — Fundada en 1827" (enlace)
- **Lado derecho:** "Vicerrectoría de Docencia" + correo `escuelaU@unicartagena.edu.co`
- **Centro inferior:** "Actualizada Junio 2026 — Escuela ETDH. Todos los derechos reservados."

---

## 9. Pendientes Post-Entrega

### 9.1. Configuración del Formulario
- **Tarea:** Implementar envío real de correos.
- **Solución propuesta:** Netlify Forms (migrando el sitio a Netlify) o Formspree.
- **Dificultad:** Baja.
- **Responsable:** Director de la Escuela ETDH.

### 9.2. Migración a Netlify
- **Tarea:** Migrar el sitio de GitHub Pages a Netlify.
- **Solución propuesta:** Netlify con despliegue continuo desde GitHub.
- **Dificultad:** Baja.
- **Responsable:** Director de la Escuela ETDH.

### 9.3. Reemplazo de Placeholders
- **Tarea:** Sustituir los archivos PDF de ejemplo con los documentos reales.
- **Ubicación:** Carpetas `documentos/poa/`, `documentos/informes/`, `documentos/riesgos/`, `documentos/organigrama/`.
- **Dificultad:** Baja.
- **Responsable:** Director de la Escuela ETDH.

### 9.4. Imágenes del Carrusel
- **Tarea:** Reemplazar los placeholders PNG con imágenes reales.
- **Ubicación:** `assets/banners/` (8 archivos).
- **Dificultad:** Baja.
- **Responsable:** Director de la Escuela ETDH.

### 9.5. Diagramas
- **Tarea:** Reemplazar los placeholders PNG con diagramas reales.
- **Ubicación:** `assets/diagramas/` (mapas conceptuales, organigrama, stack).
- **Dificultad:** Baja.
- **Responsable:** Director de la Escuela ETDH.

---

## 10. Hoja de Ruta para Migración a Netlify

### Paso 1: Crear cuenta en Netlify
1. Ir a [netlify.com](https://netlify.com).
2. Registrarse con GitHub.

### Paso 2: Conectar repositorio
1. Hacer clic en "New site from Git".
2. Seleccionar GitHub.
3. Elegir el repositorio `web-poa`.
4. Configurar rama: `main`.
5. Hacer clic en "Deploy".

### Paso 3: Configurar Netlify Forms
1. Agregar el atributo `netlify` al formulario en `index.html`:
   ```html
   <form id="form-retroalimentacion" netlify ...>
   ```
2. Subir los cambios al repositorio.
3. Netlify detectará automáticamente el formulario.

### Paso 4: Configurar notificaciones por correo
1. Ir a "Forms" en el panel de Netlify.
2. Configurar la dirección de correo para recibir las notificaciones.

### Paso 5: Configurar dominio personalizado (opcional)
1. Ir a "Domain settings" en Netlify.
2. Agregar el dominio personalizado de la Universidad.
3. Configurar los registros DNS.

---

## 11. Estructura de Archivos del Proyecto

```
web-poa/
├── index.html                     # Dashboard principal
├── poa-2025.html                  # Detalle POA 2025
├── poa-2026.html                  # Detalle POA 2026
├── mapa-riesgos-2026.html         # Mapa de Riesgos 2026
├── organigrama.html               # Organigrama de la Escuela
├── stack-tecnologico.html         # Infraestructura tecnológica
├── diseno-curricular-adaptaton.html # Diseño curricular Adaptatón
├── director-etdh.html             # Funciones del Director
├── styles.css                     # Estilos globales y tokens de diseño
├── AGENTS.md                      # Reglas para asistentes IA
├── INFORME_CIERRE_PROYECTO.md     # Este documento
├── README.md                      # Documentación del proyecto
├── assets/
│   ├── logo/
│   │   └── logo_oficial.png       # Logo institucional
│   ├── icons/
│   │   └── linkedin.svg           # Icono de LinkedIn
│   ├── banners/                   # Imágenes del carrusel (8)
│   └── diagramas/                 # Mapas conceptuales y diagramas
├── docs/
│   └── context/
│       ├── PRD.md
│       ├── ESTILO.md
│       ├── TARGET.md
│       ├── HISTORIAS.md
│       └── REFERENCIA_FUNCIONES.md
└── documentos/
    ├── poa/
    │   ├── POA_2025_v1.0.pdf
    │   └── POA_2026_v1.0.pdf
    ├── informes/
    │   ├── actividades/           # Informes por actividad
    │   │   └── *.pdf             # (18 informes)
    │   ├── diagnostico-ETDH.pdf
    │   ├── hoja-ruta-TD.pdf
    │   ├── plan-trabajo-inicial.pdf
    │   ├── portafolio-institucional.pdf
    │   └── objetivos_desempeno/   # Informes de desempeño
    ├── riesgos/
    │   ├── mapa-riesgos-2026.pdf
    │   └── Mapa_de_Riesgos_ETDH_2025-II.pdf
    └── organigrama/
        └── organigrama-inicial.pdf
```

---

## 12. Conclusiones

El sitio web de la Escuela ETDH está completo y listo para su presentación. La estructura, el diseño, el contenido y la navegación están validados. El formulario de retroalimentación está diseñado y simulado, pendiente de configuración para envío real de correos.

**El proyecto se entrega en tiempo y forma, cumpliendo con todos los objetivos planteados.**

---

## 13. Anexos

### Anexo 1: Guía de Actualización Semestral

Para actualizar el sitio cada semestre:

1. **POA**: Modificar los datos en `poa-2025.html` y `poa-2026.html`.
2. **KPIs**: Actualizar porcentajes en `index.html` y `mapa-riesgos-2026.html`.
3. **Documentos**: Reemplazar los PDFs en las carpetas de `documentos/`.
4. **Imágenes**: Reemplazar los placeholders en `assets/banners/` y `assets/diagramas/`.
5. **Funciones del Director**: Actualizar narrativas y roles en `director-etdh.html`.
6. **Objetivos de Desempeño**: Actualizar tabla en `poa-2025.html` y `poa-2026.html`.
7. **Footer**: Actualizar el año en el texto de derechos reservados.

### Anexo 2: Stack Tecnológico

| Capa | Tecnología |
|------|-----------|
| Frontend | HTML5 + CSS3 + JavaScript (Vanilla) |
| Framework CSS | Tailwind CSS v4 (vía CDN) |
| Iconos | Lucide Icons (vía CDN) |
| Tipografía | Roboto (Google Fonts) |
| Formulario | Pendiente (Netlify Forms recomendado) |
| Hosting | GitHub Pages (actual) → Netlify (recomendado) |
