# Alonso Website - CV y Portafolio

Sitio web personal de Alonso, ingeniero de datos especializado en machine learning y análisis de datos. Construido con Astro para un rendimiento óptimo y una experiencia de usuario moderna.

## 🚀 Características

- **CV Profesional**: Sección de experiencia, habilidades y logros
- **Portafolio de Proyectos**: Showcase de proyectos de ingeniería de datos
- **Blog Técnico**: Artículos sobre data engineering, ML y mejores prácticas
- **Diseño Responsivo**: Optimizado para todos los dispositivos
- **Rendimiento Optimizado**: Construido con Astro para máxima velocidad
- **SEO Friendly**: Meta tags y estructura optimizada para motores de búsqueda

## 🛠️ Tecnologías

- **Astro**: Framework web moderno y rápido
- **TypeScript**: Tipado estático para mejor desarrollo
- **CSS**: Estilos personalizados sin dependencias externas
- **PNPM**: Gestor de paquetes rápido y eficiente

## 📦 Instalación y Uso

```bash
# Instalar dependencias
pnpm install

# Iniciar servidor de desarrollo
pnpm dev

# Construir para producción
pnpm build

# Preview de la build
pnpm preview
```

## 📁 Estructura del Proyecto

```
src/
├── layouts/
│   └── Layout.astro          # Layout principal
├── pages/
│   ├── index.astro           # Página de inicio
│   ├── blog/
│   │   ├── index.astro       # Lista de posts del blog
│   │   └── [slug].astro      # Páginas individuales de posts
│   ├── proyectos.astro       # Portafolio de proyectos
│   └── contacto.astro        # Página de contacto
└── public/
    └── favicon.svg           # Favicon
```

## 🎨 Personalización

### Contenido
- **CV**: Edita `src/pages/index.astro` para actualizar experiencia y habilidades
- **Proyectos**: Modifica `src/pages/proyectos.astro` para agregar tus proyectos
- **Blog**: Añade nuevos posts en `src/pages/blog/[slug].astro`
- **Contacto**: Actualiza información de contacto en `src/pages/contacto.astro`

### Estilos
- Los estilos están definidos en cada componente usando CSS scoped
- Colores principales: `#2563eb` (azul), `#1f2937` (gris oscuro)
- Tipografía: System fonts para mejor rendimiento

### Configuración
- **SEO**: Meta tags en `src/layouts/Layout.astro`
- **Navegación**: Links en el header del layout principal
- **Redes Sociales**: Enlaces en el footer

## 🚀 Despliegue

El sitio está optimizado para despliegue estático. Puedes desplegarlo en:

- **Vercel**: `vercel --prod`
- **Netlify**: Arrastra la carpeta `dist/` después de `pnpm build`
- **GitHub Pages**: Usa GitHub Actions para build automático
- **Cualquier hosting estático**: Sube la carpeta `dist/`

## 📝 Licencia

Este proyecto es de uso personal. Siéntete libre de usarlo como inspiración para tu propio sitio web.

## 🤝 Contribuciones

Este es un proyecto personal, pero si encuentras algún error o tienes sugerencias, ¡las contribuciones son bienvenidas!

---

**Desarrollado con ❤️ usando Astro**