# BravoDesign — The Glitch Constructivist

Sitio web y portafolio de diseño de Tomás Bravo con estética constructivista, Neo-Memphis ética y arquitectura SEO para alto rendimiento.

## 🚀 Vista Previa Rápida

Puedes abrir directamente el archivo `index.html` en tu navegador favorito, o iniciar un servidor local con Python:

```bash
python -m http.server 8000
```

Luego abre tu navegador en [http://localhost:8000](http://localhost:8000).

## 📁 Estructura del Proyecto

- `index.html`: Página principal del portafolio con enlaces directos a los casos de estudio.
- `proyecto-template.html`: **Plantilla maestra reutilizable** para publicar nuevos casos de estudio y proyectos con SEO técnico y diseño responsive.
- `proyectos/`: Directorio de publicaciones de proyectos individuales:
  - `signia-seo-web-design.html`: Caso de estudio de rediseño web y posicionamiento orgánico.
  - `nam-landing-page.html`: Caso de estudio de landing page de alta conversión (CRO).
  - `gocards-marketplace-tcg.html`: Caso de estudio del marketplace e-commerce con filtros avanzados.
- `assets/projects/`: Imágenes y mockups optimizados de cada proyecto.
- `sitemap.xml`: Mapa del sitio XML jerárquico para indexación en Google.
- `robots.txt`: Directivas para motores de búsqueda.
- `DESIGN.md`: Especificación de tokens de diseño, paleta de colores y tipografía.

## 🌐 Publicación en GitHub Pages

1. Inicializa el repositorio Git:
   ```bash
   git init
   git add .
   git commit -m "feat: portfolio with complete project templates and SEO optimization"
   ```
2. Conecta con tu repositorio en GitHub:
   ```bash
   git branch -M main
   git remote add origin https://github.com/Tbravop/bravodesign.git
   git push -u origin main
   ```
3. En la configuración de tu repositorio en GitHub (**Settings > Pages**), selecciona la rama `main` y la carpeta `/ (root)` para publicar tu sitio web.
