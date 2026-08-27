# Candidatura — Bootcamp Intensivo de IA

Micro-site de candidatura de **José Galindo** para un Bootcamp Intensivo de IA. Página única (single-page), autocontenida, sin dependencias de build ni frameworks: un solo archivo `index.html` con CSS y JS inline, listo para servirse como sitio estático.

**Demo:** https://josegalindoegea-devlpr.github.io/candidatura-bootcamp-ia/
*(activo en cuanto se habilite GitHub Pages en este repositorio — ver [Despliegue](#despliegue))*

Preview alternativa (mientras se despliega Pages): https://claude.ai/code/artifact/55eb4976-0a11-42b4-86e7-2239c2f89f56

## Contenido

El site cubre, en cinco secciones de scroll:

1. **Hero** — titular de posicionamiento y accesos directos a LinkedIn / GitHub.
2. **Motivación** — por qué este bootcamp, en vez de seguir consumiendo teoría por libre.
3. **Qué aporto** — rigor y metodología, mentalidad builder, colaboración y resiliencia.
4. **Proyecto** — propuesta de arquitectura propia: un agente de gobierno de SLAs y reporting ejecutivo (RAG + modelo + orquestación), con diagrama de la arquitectura conceptual.
5. **Cierre** — llamada a la acción con LinkedIn, GitHub y contacto directo.

## Stack técnico

- HTML5 + CSS3 (custom properties, grid/flexbox) + JavaScript vanilla — sin librerías ni build step.
- Tipografías: [Syne](https://fonts.google.com/specimen/Syne), [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans) e [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) vía Google Fonts.
- Diagrama de arquitectura en SVG nativo (sin librerías de diagramado).
- Tema claro/oscuro automático según preferencia del sistema (`prefers-color-scheme`).
- Accesibilidad: navegación por teclado con foco visible, `prefers-reduced-motion` respetado, textos alternativos en el diagrama.

## Ejecutar en local

No requiere instalación. Basta con abrir el archivo directamente:

```bash
git clone https://github.com/josegalindoegea-devlpr/candidatura-bootcamp-ia.git
cd candidatura-bootcamp-ia
open index.html   # macOS — en Linux: xdg-open index.html · en Windows: start index.html
```

O sirviéndolo con cualquier servidor estático, por ejemplo:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Despliegue

El repositorio está preparado para publicarse con **GitHub Pages** directamente desde `main`:

1. Ve a **Settings → Pages**.
2. En **Source**, selecciona **Deploy from a branch**.
3. Elige la rama `main` y la carpeta `/ (root)`.
4. Guarda. En 1–2 minutos el site queda disponible en:
   `https://josegalindoegea-devlpr.github.io/candidatura-bootcamp-ia/`

## Estructura del repositorio

```
candidatura-bootcamp-ia/
├── index.html   # Site completo (HTML + CSS + JS inline)
└── README.md    # Este documento
```

## Contacto

- LinkedIn: [linkedin.com/in/josegalindo](https://www.linkedin.com/in/josegalindo/)
- GitHub: [github.com/josegalindoegea-devlpr](https://github.com/josegalindoegea-devlpr)
- Email: jose.galindo.egea@gmail.com
