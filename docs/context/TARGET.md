# TARGET.md 

## Escuela ETDH · Sitio Web de Seguimiento y Gestión

**Proyecto:** Sitio Web de Seguimiento de la Escuela de Educación para el Trabajo y el Desarrollo Humano (ETDH)  
**Versión:** 1.0  
**Estado:** Genotype Definition  
**Fecha:** 16 de junio de 2026  
**Responsable:** Dirección de la Escuela ETDH — Vicerrectoría de Docencia, Universidad de Cartagena  
**Metodología:** Desarrollo Guiado por Contexto (DGC)

---

## **0\. Declaración de Arquetipo**

El sitio web de la Escuela ETDH es un **Maestro de Obras que muestra los planos y el avance de la construcción**.

No es un vendedor, ni un narrador, ni un anfitrión. Es un **constructor** que tiene los planos abiertos sobre la mesa, el cronograma a la vista, y los materiales organizados. No promete lo que no tiene. Muestra lo que ha hecho, lo que está haciendo, y lo que necesita para avanzar.

Su tono no es de celebración ni de disculpa. Es de **informe técnico honesto**. Dice: "Esto es lo que hemos construido. Esto es lo que falta. Aquí están los planos. Usted juzgue."

**Filosofía de Conversión:** Participación Ciudadana. El objetivo no es vender ni convencer. Es **invitar a contribuir** a la construcción de la Escuela, desde la transparencia radical.

---

## **1\. El Modelo de Conversión (Purpose Patterns)**

### **1.1. Driver (Motor Emocional)**

El usuario no viene a comprar ni a entretenerse. Viene a **verificar**, a **entender** y, potencialmente, a **aportar**.

| Emoción | Cómo se activa | Cómo se usa |
| :---- | :---- | :---- |
| **Confianza** | Mostrando datos duros, documentos verificables y avances reales. | La transparencia genera confianza. No se ocultan los riesgos. |
| **Pertinencia** | Mostrando la conexión con el territorio, las vocaciones productivas y las necesidades de Cartagena. | El usuario siente que esto le importa. |
| **Curiosidad** | Invitando a explorar los documentos, los KPIs y los riesgos. | El usuario quiere entender cómo funciona. |
| **Responsabilidad** | Mostrando lo que falta y los riesgos. | El usuario siente que puede contribuir a resolverlo. |

### **1.2. Mecánica de CTA (Call to Action)**

| Tipo de CTA | Texto | Ubicación |
| :---- | :---- | :---- |
| **Primario** | "Contribuir a este proceso" | Al final de cada página, junto a los KPIs de riesgo. |
| **Secundario** | "Ver detalle del POA" | En la tabla de actividades. |
| **Terciario** | "Descargar informe completo" | Junto a cada actividad. |

### **1.3. Estrategia de Participación**

El formulario de retroalimentación no es un "contacto comercial". Es una **invitación a la construcción colectiva**.

- El usuario no es un "cliente". Es un **ciudadano que aporta** a la construcción de la Escuela.  
- El mensaje no es "déjanos tus datos". Es **"¿quieres contribuir a este proceso?"**.  
- El tono no es "esperamos tu mensaje". Es **"tu aporte es parte de los cimientos"**.

---

## **2\. Física del Comportamiento (Timing & Motion)**

### **2.1. Ritmo Cardíaco del Alma**

El Alma define la intención psicológica. El Cuerpo (`ESTILO.md`) define los valores técnicos (los tokens de duración). Esta sección establece **cuándo** debe aplicarse cada ritmo.

| Ritmo | Duración (Referencia al Cuerpo) | Uso | Sensación |
| :---- | :---- | :---- | :---- |
| **Diálogo Ciudadano** | `--duration-medium` (350ms) | Aparición de tarjetas, transiciones de secciones, carga de KPIs. | Pausado, reflexivo, humano. |
| **Respuesta Técnica** | `--duration-fast` (200ms) | Hover de botones, feedback de interacción, enlaces. | Eficiente, preciso, sin demora. |
| **Carga de Datos** | `--duration-slow` (600ms) | Aparición de elementos complejos (tablas, gráficos). | Muestra que la información está siendo procesada. |
| **Estado de Espera** | `--duration-medium` (350ms) | Cuando se envía el formulario. | Comunica que el mensaje está viajando. |

### **2.2. Curvas de Comportamiento**

| Curva (Referencia al Cuerpo) | Uso | Sensación |
| :---- | :---- | :---- |
| `--ease-glass` | Aparición de tarjetas y paneles. | Suave, como vidrio flotando. |
| `--ease-tactile` | Feedback de botones e interacciones. | Respuesta rápida, precisa. |
| `--ease-organic` | Carga de elementos complejos. | Natural, humano. |

### **2.3. Micro-Interacciones**

| Acción | Comportamiento | Sensación |
| :---- | :---- | :---- |
| **Pasar cursor sobre tarjeta** | Elevación (translateY \-4px), sombra más intensa. | La información se acerca al usuario. |
| **Pasar cursor sobre botón** | Elevación (-2px), brillo (brightness). | El botón responde como un objeto físico. |
| **Enviar formulario** | Botón cambia a "Enviando..." con animación de carga. | El sistema reconoce y procesa el aporte. |
| **Carga de página** | Aparición secuencial de elementos (fade-in con stagger). | La información se revela con orden. |

---

## **3\. Ingeniería de la Voz (Micro-Copywriting)**

### **3.1. El Arquetipo de Voz**

La voz del sitio es la de un **Maestro de Obras Honesto**.

| Atributo | Descripción |
| :---- | :---- |
| **Tono** | Directo, informativo, sin rodeos. |
| **Estilo** | Oraciones completas pero sin florituras. Hechos, no opiniones. |
| **Actitud** | Transparente: muestra los riesgos y los avances por igual. |
| **Relación con el usuario** | El usuario no es un cliente, es un **veedor** o **colaborador**. |

### **3.2. Matriz de Voz**

| Estado | Tono | Ejemplo (Texto Real) |
| :---- | :---- | :---- |
| **Neutral (Instrucción)** | Directo, descriptivo. | "Esta página muestra los avances en la construcción de la Escuela ETDH." |
| **Éxito (Confirmación)** | Informativo, sin celebración excesiva. | "Actividad completada. Documentos disponibles para consulta." |
| **Error (Fricción)** | Honesto, sin disculpas. | "Actividad bloqueada. Pendiente de resolución de normativa interna." |
| **Espera (Carga)** | Informativo, procesual. | "Cargando datos del POA 2026..." |
| **Invitación (CTA)** | Directa, colaborativa. | "¿Quieres contribuir a este proceso?" |
| **Confirmación de envío** | Agradecida, pero sin exageración. | "Gracias por tu aporte. Hemos recibido tu mensaje." |

### **3.3. Micro-Copy Específico por Componente**

| Componente | Texto | Justificación |
| :---- | :---- | :---- |
| **Título del sitio** | "Escuela ETDH — Universidad de Cartagena" | Institucional, directo. |
| **Subtítulo del sitio** | "Seguimiento y gestión del proceso de construcción" | Describe exactamente lo que es. |
| **Etiqueta del botón principal** | "Contribuir a este proceso" | Invita a la participación, no a la compra. |
| **Etiqueta de descarga de PDF** | "Descargar informe completo" | Directo, funcional. |
| **Etiqueta de actividad bloqueada** | "Bloqueada — Pendiente de resolución" | Honesto, sin rodeos. |
| **Etiqueta de actividad completada** | "Completada — Documentos disponibles" | Informativo, sin celebración. |
| **Título del Mapa de Riesgos** | "Riesgos identificados y planes de mitigación" | Transparente. |
| **Título del formulario** | "Aporta a la construcción de la Escuela ETDH" | Conecta con el arquetipo del Maestro de Obras. |
| **Placeholder del mensaje** | "¿Qué quieres aportar o preguntar?" | Invita a la reflexión. |
| **Mensaje de carga del formulario** | "Enviando tu aporte..." | Procesual, informativo. |
| **Mensaje de éxito del formulario** | "Gracias por tu contribución." | Agradece, pero no exagera. |

### **3.4. Textos para Estados Vacíos (Empty States)**

| Contexto | Texto | Justificación |
| :---- | :---- | :---- |
| **Sin documentos disponibles** | "No hay documentos disponibles para esta actividad." | Honesto, directo. |
| **Sin actividades en esta categoría** | "No hay actividades registradas en este objetivo." | Informativo. |
| **Sin riesgos en esta categoría** | "No hay riesgos identificados en esta categoría." | Informativo. |

### **3.5. Reglas de Sintaxis**

| Regla | Ejemplo (Correcto) | Ejemplo (Incorrecto) |
| :---- | :---- | :---- |
| **Oraciones completas pero breves** | "Esta actividad está en proceso." | "Estamos trabajando en esto y esperamos tenerlo listo pronto." |
| **Sin exclamaciones** | "Actividad completada." | "¡Actividad completada\!" |
| **Sin preguntas retóricas** | "Descarga el informe completo." | "¿No te gustaría descargar el informe?" |
| **Sin jerga excesiva** | "Pendiente de resolución normativa." | "Pendiente de sinergia interinstitucional para la optimización de procesos." |
| **Sin lenguaje de ventas** | "Conoce los avances." | "Descubre el futuro de la educación en Cartagena." |

### **3.6. Prohibiciones de Voz (Anti-Patrones Verbales)**

| \# | Prohibición | Razón |
| :---- | :---- | :---- |
| 1 | ❌ **Sarcasmo o ironía** | Inapropiado para una institución pública. |
| 2 | ❌ **Exclamaciones** | Rompe la sobriedad del tono. |
| 3 | ❌ **Lenguaje de marketing** | "Revolucionario", "transformador", "increíble". |
| 4 | ❌ **Disculpas excesivas** | "Lamentamos los inconvenientes", "Pedimos disculpas". |
| 5 | ❌ **Lenguaje técnico inaccesible** | Sin explicación para el ciudadano. |
| 6 | ❌ **Lenguaje infantil o simplista** | Subestima al usuario. |
| 7 | ❌ **Adjetivos emocionales sin soporte** | "Excelente", "maravilloso", "espectacular". |
| 8 | ❌ **Órdenes directas** | "Haz clic aquí", "Descarga ahora". Usar invitaciones suaves. |

---

## **4\. Prompts de Inyección (El "Virus" de Contexto)**

### **4.1. Prompt de Activación del Alma**

Cuando se genere nuevo código, la IA debe cargar este TARGET.md para asegurar que los textos, ritmos y comportamientos sean consistentes.

**ACTIVA EL GENOTIPO:**

Este sitio web es un **Maestro de Obras Honesto**. Su voz es directa, informativa y transparente. No usa lenguaje de marketing, ni sarcasmo, ni exclamaciones. Informa los avances y los riesgos con la misma claridad.

**Reglas de comportamiento:**

- Los textos deben ser directos y breves.  
- Los estados de éxito no celebran, informan.  
- Los estados de error no piden disculpas, describen el problema.  
- El CTA principal es "Contribuir a este proceso", no "Contáctanos".

**Prohibiciones absolutas:**

- No usar exclamaciones.  
- No usar lenguaje de ventas.  
- No usar sarcasmo.  
- No usar órdenes directas ("haz clic aquí").

Aplica este genotipo a todos los textos, interacciones y ritmos del sitio.

---

## **5\. Checklist de Validación del Alma**

- [ ] El arquetipo de "Maestro de Obras" está claro y es consistente.  
- [ ] Los KPIs de conversión están definidos (participación, no venta).  
- [ ] Los ritmos de comportamiento están alineados con el arquetipo (diálogo ciudadano).  
- [ ] La matriz de voz cubre todos los estados (neutral, éxito, error, espera, CTA).  
- [ ] Los textos son directos, informativos y sin exclamaciones.  
- [ ] Las prohibiciones verbales están claras.  
- [ ] El prompt de inyección está redactado.

