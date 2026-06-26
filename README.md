# Escuela ETDH — Sitio Web de Seguimiento y Gestión

Sitio web institucional de la Escuela de Educación para el Trabajo y el Desarrollo Humano (ETDH) de la Universidad de Cartagena. Funciona como tablero de control de gestión que comunica de manera transparente el estado de avance de la creación y puesta en marcha de la Escuela.

No es una página de marketing. Busca informar, rendir cuentas y recibir retroalimentación de la comunidad.

## Estructura del Proyecto

```
web-poa/
├── index.html                     # Dashboard principal
├── poa-2025.html                  # Detalle POA 2025
├── poa-2026.html                  # Detalle POA 2026
├── mapa-riesgos-2026.html         # Mapa de Riesgos 2026
├── documentos.html                # Repositorio de documentos
├── organigrama.html               # Organigrama de la Escuela
├── stack-tecnologico.html         # Infraestructura tecnológica
├── styles.css                     # Estilos globales y tokens de diseño
├── AGENTS.md                      # Reglas para asistentes IA
├── assets/
│   ├── logo/
│   │   └── logo-u-blanco.svg      # Logo institucional
│   ├── banners/                   # Imágenes del carrusel (8)
│   └── diagramas/                 # Mapas conceptuales y diagramas
├── docs/
│   └── context/
│       ├── PRD.md                 # Documento de Requisitos de Producto
│       ├── ESTILO.md              # Sistema de diseño y tokens visuales
│       ├── TARGET.md              # Arquetipo de voz y comportamiento
│       └── HISTORIAS.md           # Backlog de historias de usuario
├── documentos/                    # PDFs institucionales
│   ├── diagnostico-ETDH-UdeC.pdf
│   ├── hoja-ruta-TD-ETDH.pdf
│   ├── plan-trabajo-inicial.pdf
│   ├── portafolio-institucional.pdf
│   ├── poa-2025-completo.pdf
│   ├── poa-2026-completo.pdf
│   ├── mapa-riesgos-2026-completo.pdf
│   └── informes/                  # Informes por actividad
└── README.md
```

## Tecnologías Utilizadas

| Capa | Tecnología |
|------|-----------|
| Marcado | HTML5 (semántico) |
| Estilos | CSS3 + Tailwind CSS v4 (vía CDN) |
| Tipografía | Roboto (Google Fonts) |
| Iconos | Lucide Icons (vía CDN) |
| Interactividad | JavaScript (Vanilla) |
| Hosting | Servidor institucional o GitHub Pages |

## Metodología

Este proyecto se desarrolla bajo **Desarrollo Guiado por Contexto (DGC)**, una metodología que utiliza cuatro archivos de contexto como fuente única de verdad:

- [PRD.md](docs/context/PRD.md) — visión, alcance, restricciones y modelo de datos
- [ESTILO.md](docs/context/ESTILO.md) — sistema de diseño, tokens visuales, componentes
- [TARGET.md](docs/context/TARGET.md) — arquetipo de voz (Maestro de Obras Honesto)
- [HISTORIAS.md](docs/context/HISTORIAS.md) — backlog evolutivo de historias de usuario

Cada historia de usuario se trabaja una a la vez siguiendo el protocolo de destilación: cargar ADN, planificar, codificar, auditar y consolidar.

## Instalación y Uso

1. Clona el repositorio:
   ```bash
   git clone <url-del-repositorio>
   cd web-poa
   ```

2. Abre `index.html` en tu navegador:
   ```bash
   open index.html
   ```

No requiere servidor web, compilación ni instalación de dependencias. El sitio funciona completamente desde el sistema de archivos local.

## Actualización de Contenido

- **Periodicidad:** semestral (junio y diciembre).
- **Formato:** cada actualización genera una nueva versión de los archivos HTML.
- **Responsable:** Dirección de la Escuela ETDH.
- **Documentos:** los PDFs se actualizan en la carpeta `documentos/`.

Para actualizar:
1. Modifica los datos en los archivos HTML correspondientes.
2. Reemplaza los PDFs en `documentos/` con las nuevas versiones.
3. Reemplaza las imágenes en `assets/banners/` y `assets/diagramas/` según corresponda.
4. Actualiza los archivos de contexto en `docs/context/` si el alcance cambia.

## Accesibilidad

El sitio cumple con los estándares WCAG AA:
- Contraste mínimo 4.5:1 en todos los textos
- Navegación por teclado (Tab, Enter, Espacio)
- Skip link para saltar el menú de navegación
- Atributos ARIA en elementos interactivos
- `prefers-reduced-motion` respetado
- Legible con zoom al 200%

## Créditos

**Universidad de Cartagena** — Fundada en 1827

Vicerrectoría de Docencia
Dirección de la Escuela de Educación para el Trabajo y el Desarrollo Humano (ETDH)

Contacto: [escuelaU@unicartagena.edu.co](mailto:escuelaU@unicartagena.edu.co)
