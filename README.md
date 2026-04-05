# InnovaDigital — Blog de Transformación Digital

Blog profesional sobre innovación y transformación digital para industrias.

## Estructura del proyecto

```
innovadigital/
├── index.html              ← El blog principal
├── admin/
│   └── index.html          ← Panel de administración
├── content/
│   └── noticias.json       ← Base de datos de artículos
├── netlify.toml            ← Configuración de Netlify
└── .gitignore
```

## Cómo publicar un artículo

1. Abrí `/admin/index.html` en tu navegador
2. Hacé clic en "Nuevo artículo"
3. Completá el formulario y guardá
4. Se descargará automáticamente el archivo `noticias.json`
5. Reemplazá el archivo `content/noticias.json` con el descargado
6. Subí los cambios a GitHub:
   ```
   git add content/noticias.json
   git commit -m "Nuevo artículo"
   git push
   ```
7. Netlify actualiza el blog automáticamente en 1-2 minutos

## Deploy en Netlify

1. Creá una cuenta en [netlify.com](https://netlify.com)
2. "Add new site" → "Import an existing project"
3. Conectá tu repositorio de GitHub
4. Build settings: dejá todo en blanco (es HTML estático)
5. Hacé clic en "Deploy site"

## Tecnologías

- HTML + CSS + JavaScript puro (sin frameworks)
- Netlify para hosting y deploy automático
- GitHub para control de versiones
- JSON como base de datos de artículos
