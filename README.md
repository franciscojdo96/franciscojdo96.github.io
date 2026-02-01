# Portafolio profesional de Data Science y Riesgo

Este repositorio contiene un portafolio y blog profesional orientado a roles de **Data Science**, **Analytics** y **gestión de riesgo financiero**. El objetivo del sitio es transmitir capacidad analítica, criterio de negocio y un impacto cuantificable a reclutadores y líderes de la industria.

## 📦 Arquitectura elegida

- **GitHub Pages + Jekyll**: GitHub Pages ofrece alojamiento gratuito para sitios estáticos y utiliza Jekyll para convertir archivos Markdown en páginas web【702654868471171†L84-L90】. Esto permite editar posts o proyectos en Markdown sin depender de frameworks pesados, cumpliendo con la restricción de simplicidad.
- **Jekyll sin tema predefinido**: se creó un tema personalizado con HTML y CSS limpio. De esta forma evitamos sobre‑ingeniería y logramos un diseño moderno, minimalista y orientado a fintech.
- **Colección personalizada de proyectos**: se definió una colección `projects` en `_config.yml` que permite crear páginas de proyectos en la carpeta `_projects` y listarlas automáticamente en la página principal y en `/projects/`.

## 🗂️ Estructura del repositorio

```
portfolio-site/
├── _config.yml            # Configuración de Jekyll y colección de proyectos
├── _includes/             # Componentes reutilizables (navbar y footer)
├── _layouts/              # Plantillas base, post y proyecto
├── _projects/             # Proyectos individuales en formato Markdown
│   └── proyecto-ejemplo.md
├── _posts/                # Entradas de blog (formato YYYY-MM-DD-titulo.md)
│   └── 2026-01-01-ejemplo-post.md
├── assets/
│   └── css/style.css      # Estilos modernos y responsivos
├── index.html             # Página de inicio con hero, impacto, proyectos y blog
├── projects/index.html    # Índice de proyectos
├── blog/index.html        # Índice del blog
└── README.md              # Esta guía
```

### Convenciones de proyectos y posts

- **Proyectos (`_projects`)**: cada proyecto es un archivo Markdown con front matter (encabezado YAML) que incluye campos como `title`, `date`, `industry`, `role`, `metrics`, `summary`, `context`, `problem`, `solution`, `impact` y `links`. El layout `project.html` usa estos campos para crear una página detallada. La estructura Problem → Contexto → Solución → Impacto sigue el marco de storytelling recomendado【954677612423152†L165-L176】.
- **Posts (`_posts`)**: los posts viven en la carpeta `_posts` y su nombre debe seguir el patrón `AAAA-MM-DD-titulo.md`【503799039210328†L37-L44】. Cada post debe empezar con front matter indicando `layout: post`, `title`, `date`, `categories` y `tags`【503799039210328†L49-L56】. El contenido se escribe en Markdown.

## 🧭 Mapa de navegación

- **Inicio** (`/`): sección principal con hero, métricas de impacto, proyectos destacados y últimas entradas del blog.
- **Proyectos** (`/projects/`): lista completa de proyectos, cada uno con tarjeta resumida y enlace a su página de detalle.
- **Blog** (`/blog/`): todas las entradas del blog, ordenadas de más reciente a más antigua.

La navegación se implementa mediante una barra superior sencilla y sticky, con colores corporativos.

## 🎨 Diseño orientado a reclutador

El diseño utiliza una paleta de colores inspirada en fintech (azules profundos y acentos turquesa) y tipografía moderna. Los componentes clave son:

- **Hero section**: resume la propuesta de valor en una frase contundente y una llamada a la acción. Este elemento ayuda a captar la atención en segundos.
- **Sección de impacto**: destaca métricas clave (por ejemplo, mejoras porcentuales o ahorros en millones) para evidenciar resultados cuantificables【954677612423152†L165-L176】. Puedes personalizar estos datos acorde a tus logros.
- **Tarjetas de proyectos**: muestran el título, fecha, industria, resumen e invitan a “Ver detalles”. El diseño es responsivo y utiliza transiciones sutiles.
- **Blog técnico‑profesional**: listado claro de posts con fecha y resumen. Está pensado para artículos que combinen análisis técnico con aplicaciones de negocio【994322482176338†L83-L105】.

### Estructura recomendada de proyectos (storytelling)

1. **Contexto** – Describe la industria, el producto o servicio y el tamaño del problema. Sitúa al lector en el escenario adecuado【954677612423152†L165-L176】.
2. **Problema** – Define qué se quería optimizar (churn, fraude, riesgo crediticio) y por qué los métodos existentes fallaban【954677612423152†L199-L206】.
3. **Solución técnica** – Explica cómo abordaste el problema: métodos de análisis, selección de modelos, ingeniería de variables, validación y herramientas utilizadas.
4. **Impacto cuantificado** – Traducir métricas técnicas en resultados de negocio: porcentaje de mejora, ahorro en costes o incremento en ingresos【954677612423152†L229-L235】.
5. **Recursos** – Opcionalmente enlaza al repositorio, dashboards, presentaciones o publicaciones derivadas.

### Guía para escribir posts estratégicos

Los posts del blog no deben ser meramente tutoriales; deben demostrar criterio de negocio y pensamiento crítico. Sigue estos consejos:

- Elige temas alineados con tu rol objetivo y tu industria. Los proyectos con relevancia real superan a los ejemplos genéricos【994322482176338†L85-L90】.
- Presenta un **caso práctico**: comienza describiendo el problema y su importancia para la empresa o sector【994322482176338†L102-L105】.
- Explica la **metodología** y **razona** tus decisiones técnicas. Menciona por qué elegiste ciertos algoritmos o métricas y qué alternativas descartaste.
- Cuantifica el **impacto** siempre que sea posible: incrementos en métricas, reducciones de costes o mejoras en experiencia de usuario【954677612423152†L229-L235】.
- Finaliza con un **aprendizaje personal** o recomendación para otros profesionales.

## 🚀 Paso a paso para desplegar en GitHub Pages

Sigue estos pasos para publicar tu portafolio:

1. **Crear el repositorio**: en GitHub, crea un nuevo repositorio público llamado `usuario.github.io` (el prefijo debe coincidir exactamente con tu usuario【552211172130822†L24-L29】). Si prefieres un sub‑sitio (por ejemplo, `portfolio`), puedes nombrarlo de otra forma y la URL será `usuario.github.io/nombre`【702654868471171†L123-L129】.
2. **Clonar el repositorio**: clona el repositorio en tu máquina con `git clone https://github.com/usuario/usuario.github.io`【552211172130822†L46-L52】.
3. **Copiar el contenido**: copia la carpeta `portfolio-site` en la raíz del repositorio clonado y confirma que la estructura (carpetas y archivos) se mantenga.
4. **Agregar, confirmar y subir cambios**: ejecuta `git add .`, `git commit -m "Initial portfolio"` y `git push origin main`【552211172130822†L98-L107】. Alternativamente, utiliza la interfaz web para subir los archivos y hacer un commit.
5. **Activar GitHub Pages**: en la configuración del repositorio, ve a la sección **Pages**, selecciona la rama `main` y la carpeta raíz como fuente de publicación y guarda los cambios【702654868471171†L199-L200】. GitHub generará el sitio automáticamente.
6. **Verifica el despliegue**: una vez finalizada la acción, visita `https://usuario.github.io` para tu sitio principal o `https://usuario.github.io/portfolio` si usaste un repositorio con otro nombre【552211172130822†L116-L118】.
7. **Personaliza el dominio (opcional)**: si deseas usar un dominio propio, crea un archivo `CNAME` con tu dominio y configura los registros DNS, tal como se explica en la documentación oficial【552211172130822†L189-L200】.

### Checklist final

- [ ] Configuraste el repositorio con el nombre correcto.
- [ ] Subiste todos los archivos de esta plantilla.
- [ ] Activaste GitHub Pages en la rama `main`.
- [ ] El sitio se visualiza correctamente en desktop y móvil.
- [ ] Agregaste tus proyectos reales y posts al sitio.
- [ ] Actualizaste métricas de impacto y tu hero con tu propuesta de valor.

## 🤝 Contribuir y mantenimiento

Este sitio está diseñado para ser extensible a largo plazo. Añade nuevos proyectos creando archivos en `_projects/` y nuevos posts en `_posts/`. El CSS se encuentra en `assets/css/style.css` y puedes modificar variables de color o tipografía para ajustar la identidad visual.

Para obtener más información sobre cómo escribir posts o personalizar Jekyll, consulta la documentación oficial【503799039210328†L30-L52】. Si experimentas con otras configuraciones o deseas agregar paginación, etiquetas o búsqueda, te recomendamos revisar los recursos de Jekyll y la guía de GitHub Pages【552211172130822†L189-L193】.

¡Éxito en la construcción de tu marca profesional!