# [PRD.md](http://PRD.md)

## Escuela ETDH · Sitio Web de Seguimiento y Gestión

**Proyecto:** Sitio Web de Seguimiento de la Escuela de Educación para el Trabajo y el Desarrollo Humano (ETDH)  
**Versión:** 1.0  
**Estado:** MVP (Producto Mínimo Viable)  
**Fecha:** 16 de junio de 2026  
**Responsable:** Dirección de la Escuela ETDH — Vicerrectoría de Docencia, Universidad de Cartagena  
**Metodología:** Desarrollo Guiado por Contexto (DGC)

---

## **1\. Visión General y Calibración**

### **1.1. Propósito Estratégico**

El sitio web debe funcionar como un **tablero de control de gestión institucional** que comunica de manera transparente el estado de avance de la creación y puesta en marcha de la Escuela de ETDH de la Universidad de Cartagena.

No es una página de marketing. No busca seducir. Busca **informar**, **rendir cuentas** y **recibir retroalimentación** de la comunidad.

### **1.2. Justificación (Contexto Estratégico)**

El diagnóstico fundacional de la ETDH en Colombia, la Región Caribe y Cartagena (Documento 1\) evidencia:

1. Un déficit estructural de calidad: más del 85% de los programas de ETDH operan sin certificación.  
2. Una tasa de informalidad en la Región Caribe que supera el 60%, haciendo que el modelo tradicional de ETDH sea inadecuado.  
3. Una brecha crítica en Cartagena: el 80% de los bachilleres no accede a educación post-media.  
4. Una fragmentación de iniciativas públicas y privadas sin articulación sistémica.

La Escuela nace para ser la **respuesta institucional** a estas brechas. El sitio web debe reflejar ese proceso de construcción con honestidad, mostrando tanto los avances como los desafíos (riesgos).

### **1.3. Objetivos del Sitio**

| Objetivo | Descripción |
| :---- | :---- |
| **Transparencia** | Mostrar el estado de ejecución del POA (2025 y 2026\) con indicadores claros y verificables. |
| **Rendición de cuentas** | Publicar los documentos soporte (actas, resoluciones, borradores) para consulta pública. |
| **Comunicación de riesgos** | Visualizar el Mapa de Riesgos y sus KPIs de monitoreo (ITNI, TPC, CAI). |
| **Participación ciudadana** | Recibir retroalimentación de la comunidad, aliados y sector productivo. |
| **Memoria institucional** | Documentar el proceso de construcción de la Escuela para futuras evaluaciones. |

### **1.4. User Personas (Arquetipos de Usuario)**

| Persona | Descripción | Necesidad Principal |
| :---- | :---- | :---- |
| **Joven cartagenero (18-25 años)** | Bachiller que busca formación técnica para insertarse en el mercado laboral. Pertenece a estratos 1-3. | Conocer la oferta formativa, fechas de inscripción y requisitos. |
| **Empresario / Gremio** | Representante del sector productivo (turismo, logística, industria) que necesita talento humano calificado. | Articular con la Escuela para definir perfiles y recibir egresados. |
| **Funcionario público** | Ministerio de Educación, Secretaría de Educación Distrital, o entes de control. | Verificar el cumplimiento normativo y el avance de la Escuela. |
| **Comunidad académica** | Docentes, investigadores y estudiantes de la Universidad de Cartagena. | Consultar los documentos fundacionales y el estado del proyecto. |
| **Aliado estratégico** | SENA, ICETEX, Cámara de Comercio, ONGs, cooperación internacional. | Identificar oportunidades de alianza y co-creación. |

---

## **2\. Alcance del Producto**

### **2.1. Funcionalidades Incluidas (MVP)**

| Funcionalidad | Descripción |
| :---- | :---- |
| **Dashboard de KPIs estratégicos** | Visualización de los 4 KPIs macro: Normativo, Metodológico, Formativo, Articulación. |
| **Detalle del POA 2025** | Tabla con objetivos, actividades, avances, estados y enlaces a informes PDF. |
| **Detalle del POA 2026** | Tabla con objetivos, actividades, avances, estados y enlaces a informes PDF. |
| **Mapa de Riesgos 2026** | Visualización de riesgos, niveles y KPIs de monitoreo (ITNI, TPC, CAI). |
| **Repositorio de documentos** | Descarga de PDFs: Diagnóstico, Hoja de Ruta TD, Portafolio, informes por actividad. |
| **Formulario de retroalimentación** | Captura de nombre, correo, organización, tipo de aporte y mensaje. |
| **Navegación jerárquica** | Tres niveles de profundidad: Dashboard → Detalle POA → Informe por actividad. |
| **Banner carrusel** | En la página de inicio, un carrusel automático con imágenes de fondo que representan los objetivos del POA 2026 y los riesgos identificados. |
| **Mapa conceptual de objetivos** | En las páginas de detalle de POA (2025 y 2026), una imagen que representa visualmente los objetivos del año. |
| **Objetivos de desempeño del director** | En las páginas de detalle de POA (2025 y 2026), un listado de las metas personales del director para ese año. |
| **Organigrama inicial** | Página o sección dedicada al organigrama inicial de la Escuela ETDH. |
| **Infraestructura tecnológica** | Página o sección dedicada a la descripción narrativa e imagen del stack tecnológico inicial de la Escuela. |

### **2.2. Exclusiones Explícitas (Anti-Patrones de Producto)**

| \# | Exclusión | Razón |
| :---- | :---- | :---- |
| 1 | **No es una página de marketing** | No hay llamados a la acción comerciales, ni mensajes de "inscríbete ahora", ni testimonios. |
| 2 | **No tiene autenticación de usuarios** | Todo el contenido es público. No hay perfiles, ni roles, ni paneles de administración. |
| 3 | **No es dinámica en tiempo real** | La actualización es semestral. La página es estática (HTML \+ CSS \+ JS). |
| 4 | **No tiene base de datos** | No se almacenan datos de usuario excepto los del formulario (que se envían por correo). |
| 5 | **No tiene comentarios públicos** | La retroalimentación es privada (formulario → correo), no hay foros ni comentarios visibles. |
| 6 | **No tiene modo oscuro** | Se prioriza la legibilidad y la institucionalidad sobre la estética experimental. |
| 7 | **No es responsive en todos los dispositivos** | Optimizada para escritorio; se garantiza legibilidad en móvil pero no experiencia completa. |
| 8 | **No tiene carrusel con imágenes reales** | Inicialmente usa placeholders; las imágenes se reemplazarán en una fase posterior. |
| 9 | **No tiene funcionalidad interactiva en el organigrama** | Es una imagen estática. |
| 10 | **No tiene funcionalidad interactiva en el mapa conceptual** | Es una imagen estática. |

### **2.3. Criterios de Aceptación Generales**

| \# | Criterio | Métrica |
| :---- | :---- | :---- |
| 1 | El dashboard muestra los 4 KPIs con barras de progreso visuales. | Sí/No |
| 2 | Cada actividad del POA tiene: nombre, avance %, tipo, fechas, síntesis y enlace a PDF. | Sí/No |
| 3 | El Mapa de Riesgos muestra los 4 riesgos con su nivel y los 3 KPIs de monitoreo. | Sí/No |
| 4 | Todos los PDFs son descargables con un solo clic. | Sí/No |
| 5 | El formulario envía correo con los datos del usuario. | Sí/No |
| 6 | La navegación de tres niveles funciona sin errores. | Sí/No |
| 7 | Todos los textos siguen el tono institucional definido en TARGET.md. | Sí/No |

---

## **3\. Stack Tecnológico (Restricción Rígida)**

### **3.1. Tecnologías Obligatorias**

| Capa | Tecnología | Justificación |
| :---- | :---- | :---- |
| **Frontend** | HTML5 \+ CSS3 \+ JavaScript (Vanilla) | Simplicidad, cero dependencias, fácil mantenimiento semestral. |
| **Framework CSS** | Tailwind CSS v4 (vía CDN) | Agilidad en el diseño, consistencia visual, tokens personalizables. |
| **Hosting** | Servidor institucional de la Universidad de Cartagena o GitHub Pages | Costo cero, control institucional. |
| **Formulario** | Formspree o EmailJS | Envío de correos sin backend. |
| **Control de versiones** | Git \+ GitHub | Trazabilidad de cambios semestrales. |

### **3.2. Tecnologías Excluidas**

| \# | Tecnología | Razón de exclusión |
| :---- | :---- | :---- |
| 1 | React / Vue / Angular | Complejidad innecesaria para una página estática. |
| 2 | Node.js / PHP / Python | No se requiere backend. |
| 3 | Base de datos (SQL / NoSQL) | No se almacenan datos. |
| 4 | CMS (WordPress, Drupal) | Mantenimiento más complejo que HTML puro. |
| 5 | Autenticación / OAuth | No hay usuarios registrados. |

---

## **4\. Estructura de Datos (Modelo de Información)**

### **4.1. Entidades Principales**

El sitio web maneja **información estructurada**, no datos transaccionales. Las entidades son:

1. **POA (Plan Operativo Anual)**: Conjunto de objetivos y actividades para un período.  
2. **Actividad**: Unidad mínima de ejecución, con indicadores y estado.  
3. **Objetivo**: Agrupador de actividades con un propósito estratégico.  
4. **Riesgo**: Amenaza identificada con probabilidad, impacto y plan de mitigación.  
5. **KPI**: Indicador clave de desempeño con valor numérico.  
6. **Documento**: Archivo PDF asociado a una actividad o al proyecto general.

### **4.2. Estructura de un POA**

{  
  "periodo": "2025",  
  "objetivos": \[  
    {  
      "id": "OBJ-01",  
      "nombre": "Diseñar el modelo operativo ágil y el ecosistema tecnológico fundacional",  
      "avance": 75,  
      "actividades": \[  
        {  
          "id": "ACT-01-01",  
          "nombre": "Mapeo y documentación de los macro-procesos misionales",  
          "avance": 75,  
          "tipo": "Producto",  
          "fecha\_inicio": "jul-25",  
          "fecha\_fin": "dic-25",  
          "responsable": "Director de la Escuela ETDH",  
          "sintesis": "Se documentaron los 3 macro-procesos clave...",  
          "documento\_pdf": "/documentos/actividad-1-1-mapeo-procesos.pdf",  
          "estado": "en\_progreso"  
        }  
      \]  
    }  
  \]  
}

### **4.3. Estructura de un Riesgo**

{  
  "id": "RIS-01",  
  "nombre": "Parálisis por Vacío Normativo Interno",  
  "probabilidad": "Muy Alta",  
  "impacto": "Crítico",  
  "nivel": "Extremo",  
  "descripcion": "Imposibilidad de registro operativo por falta de reglamentación interna...",  
  "mitigacion": "Tramitar acto administrativo interno provisional bajo figura de extensión.",  
  "kpi\_asociado": "ITNI"  
}

### **4.4. Estructura de un KPI de Riesgo**

{  
  "id": "ITNI",  
  "nombre": "Índice de Tracción Normativa Interna",  
  "valor": 80,  
  "meta": 100,  
  "descripcion": "Avance en el trámite del Acto Administrativo Interno.",  
  "frecuencia": "Mensual"  
}

---

## **5\. Arquitectura de Navegación**

### **5.1. Mapa del Sitio**

Inicio (Dashboard)  
│  
├── Banner carrusel (en index.html)  
│  
├── POA 2025  
│   ├── Resumen ejecutivo  
│   ├── Tabla de actividades  
│   ├── Mapa conceptual de objetivos  
│   └── Objetivos de desempeño del director  
│  
├── POA 2026  
│   ├── Resumen ejecutivo  
│   ├── Tabla de actividades  
│   ├── Mapa conceptual de objetivos  
│   └── Objetivos de desempeño del director  
│  
├── Mapa de Riesgos 2026  
│   ├── Resumen de riesgos  
│   └── KPIs de monitoreo  
│  
├── Documentos  
│   └── Repositorio de documentos  
│  
├── Organigrama  
│   └── Organigrama inicial de la Escuela ETDH  
│  
└── Stack Tecnológico  
    └── Infraestructura tecnológica inicial

### **5.2. Jerarquía de Información (Cinco Niveles)**

| Nivel | Contenido | Ejemplo |
| :---- | :---- | :---- |
| **1\. Dashboard** | KPIs macro, resumen por objetivos, banner carrusel, documentos. | Página de inicio. |
| **2\. Detalle de POA** | Tabla de actividades, mapa conceptual, objetivos del director. | `/poa-2025.html` |
| **3\. Informe de actividad** | Documento PDF descargable \+ síntesis ampliada. | Enlace desde la tabla. |
| **4\. Organigrama** | Imagen del organigrama inicial. | `/organigrama.html` |
| **5\. Stack Tecnológico** | Descripción e imagen del stack tecnológico inicial. | `/stack-tecnologico.html` |

---

## **6\. Reglas de Negocio**

### **6.1. Reglas de Actualización de Contenido**

| \# | Regla | Descripción |
| :---- | :---- | :---- |
| 1 | **Periodicidad semestral** | La página se actualiza dos veces al año (junio y diciembre). |
| 2 | **Versión estática** | Cada actualización genera una nueva versión de los archivos HTML. |
| 3 | **Congelación de datos** | Entre actualizaciones, los datos no cambian. |
| 4 | **Responsable único** | El Director de la Escuela ETDH es el responsable de la actualización. |

### **6.2. Reglas de Visualización de Estados**

| Estado | Símbolo | Color | Significado |
| :---- | :---- | :---- | :---- |
| Completado | \[x\] | 🟢 Verde | Actividad finalizada al 100% |
| En progreso | \[/\] | 🟡 Amarillo | Actividad entre 1% y 99% |
| Bloqueado | \[\!\] | 🔴 Rojo | Actividad detenida por falta de recursos o normativa |
| No iniciado | \[ \] | ⚪ Gris | Actividad al 0% |

### **6.3. Reglas de Acceso a Documentos**

| \# | Regla | Descripción |
| :---- | :---- | :---- |
| 1 | **Acceso público** | Todos los PDFs son descargables sin autenticación. |
| 2 | **Formato estándar** | Todos los documentos deben estar en formato PDF. |
| 3 | **Nomenclatura** | Los archivos se nombran con el formato: `actividad-XX-XX-nombre-corto.pdf` |

### **6.4. Reglas del Formulario de Retroalimentación**

| \# | Regla | Descripción |
| :---- | :---- | :---- |
| 1 | **Campos obligatorios** | Nombre, correo y mensaje. |
| 2 | **Tipo de aporte** | Selector con opciones: Sugerencia, Solicitud de alianza, Comentario, Otro. |
| 3 | **Envío por correo** | El formulario no almacena datos; envía un correo al Director. |
| 4 | **Protección de datos** | Se debe incluir un enlace a la política de protección de datos de la Universidad. |

---

## **7\. Anti-Patrones de Implementación**

### **7.1. Qué NO debe hacer la IA al generar el código**

| \# | Anti-Patrón | Razón |
| :---- | :---- | :---- |
| 1 | ❌ Usar colores hardcoded en CSS | Todos los colores deben venir de tokens en `ESTILO.md`. |
| 2 | ❌ Usar sombras negras (\#000) | Las sombras deben ser coloreadas según el sistema de diseño. |
| 3 | ❌ Generar texto en "Lorem Ipsum" | Todos los textos deben ser reales, extraídos del diagnóstico y POAs. |
| 4 | ❌ Inventar funcionalidades no especificadas | No añadir gráficos, animaciones o interacciones no solicitadas. |
| 5 | ❌ Usar dependencias externas no autorizadas | Solo Tailwind CSS y el servicio de formulario. |
| 6 | ❌ Crear páginas con diseño plano (Flat Design) | Se debe usar Glassmorphism o material definido en `ESTILO.md`. |
| 7 | ❌ Omitir la accesibilidad | Contraste mínimo 4.5:1, etiquetas ARIA, navegación por teclado. |
| 8 | ❌ Usar imágenes reales en el carrusel si no se han proporcionado | Usar placeholders claros. |
| 9 | ❌ Mezclar el menú hamburguesa con el menú horizontal | El menú hamburguesa es la navegación principal en todas las pantallas. |

### **7.2. Qué SÍ debe hacer la IA**

| \# | Práctica | Descripción |
| :---- | :---- | :---- |
| 1 | ✅ Usar tokens de `ESTILO.md` | Todos los colores, sombras y espacios deben venir de variables CSS. |
| 2 | ✅ Documentar el código | Comentarios en HTML y CSS explicando la estructura. |
| 3 | ✅ Mantener la jerarquía de tres niveles | Dashboard → Detalle → Informe. |
| 4 | ✅ Incluir footer institucional | Logo, nombre de la Universidad, Vicerrectoría, datos de contacto. |
| 5 | ✅ Usar tipografía institucional | Definida en `ESTILO.md`. |
| 6 | ✅ Enlazar todos los PDFs correctamente | Rutas relativas funcionales. |

---

## **8\. KPIs de Éxito del Sitio Web**

| \# | KPI | Métrica | Meta |
| :---- | :---- | :---- | :---- |
| 1 | **Tasa de descarga de documentos** | Número de descargas / visitantes únicos | \>20% |
| 2 | **Tasa de envío de formulario** | Número de formularios enviados / visitantes únicos | \>5% |
| 3 | **Tiempo de carga** | Tiempo hasta renderizado completo | \<2 segundos |
| 4 | **Navegación completa** | Usuarios que visitan al menos 3 páginas | \>40% |
| 5 | **Tasa de rebote** | Usuarios que salen en la primera página | \<60% |

---

## **9\. Riesgos y Dependencias**

| \# | Riesgo | Probabilidad | Impacto | Mitigación |
| :---- | :---- | :---- | :---- | :---- |
| 1 | **Cambio de prioridades institucionales** | Media | Alto | El sitio debe ser fácilmente actualizable; los datos son estáticos. |
| 2 | **Falta de documentos PDF finalizados** | Alta | Alto | Priorizar la publicación de documentos existentes; los pendientes se añaden en la siguiente versión. |
| 3 | **Problemas con el servicio de formulario** | Baja | Medio | Tener un correo de respaldo ([escuelaU@unicartagena.edu.co](mailto:escuelaU@unicartagena.edu.co)). |
| 4 | **Obsolescencia de Tailwind CDN** | Baja | Medio | Fijar la versión específica en el CDN. |

---

## **10\. Header y Navegación**

### **10.1. Header**

- **Logo:** Logo "U" en contorno blanco al lado izquierdo.
- **Separador:** Línea vertical delgada gris claro.
- **Texto:** "Escuela ETDH".
- **Menú:** Menú hamburguesa siempre visible en el lado izquierdo.

### **10.2. Menú Hamburguesa**

- **Comportamiento:** Panel lateral izquierdo que se despliega al hacer clic. Empuja el contenido principal hacia la derecha.
- **Enlaces:** Inicio, POA 2025, POA 2026, Mapa de Riesgos, Documentos, Organigrama, Stack Tecnológico.
- **Siempre visible:** En todas las pantallas (no solo en móviles).

---

## **11\. Checklist de Validación del PRD**

- [ ] El propósito y la justificación están alineados con el diagnóstico y los POAs.  
- [ ] Las user personas reflejan los públicos reales del proyecto.  
- [ ] Las exclusiones explícitas son claras y están justificadas.  
- [ ] El stack tecnológico está definido y es realista.  
- [ ] El modelo de datos cubre toda la información a mostrar.  
- [ ] La arquitectura de navegación tiene tres niveles de profundidad.  
- [ ] Las reglas de negocio son accionables y verificables.  
- [ ] Los anti-patrones evitan que la IA "alucine" funcionalidades.  
- [ ] Los KPIs de éxito son medibles.  
- [ ] Los riesgos tienen mitigaciones viables.

