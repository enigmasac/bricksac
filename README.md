# BRICK Proyectos & Construcción S.A.C.

Landing page corporativa para BRICK, empresa peruana de ingeniería, arquitectura y construcción con más de 24 años de trayectoria.

## Stack Técnico

- **HTML5** semántico
- **Tailwind CSS** (CDN) + config modular
- **Alpine.js** para interactividad
- **Font Awesome** iconos
- **Google Fonts** (Inter)

## Estructura

```
web/
├── index.html          # Single page principal
├── css/
│   └── styles.css      # Estilos personalizados
├── js/
│   └── tailwind.config.js  # Config de Tailwind
└── assets/
    ├── logo.png
    ├── logo-v2.png
    ├── logo-v3.png
    ├── hero-video.mp4      # NO en git (ver .gitignore)
    └── projects/           # NO en git (ver .gitignore)
        └── *.jpg
```

## Archivos excluidos de Git

El `.gitignore` excluye multimedia pesada:
- `assets/hero-video.mp4` (~11MB)
- `assets/projects/` (~3.5MB de imágenes)

Estos archivos se mantienen solo en el servidor y en local.

## Deploy

```bash
# 1. Comprimir (sin multimedia)
tar -czvf deploy.tar.gz --exclude='.git' --exclude='assets/hero-video.mp4' --exclude='assets/projects' .

# 2. Subir al servidor
scp deploy.tar.gz bricksac@serverenigma.com:~/

# 3. Descomprimir en servidor
ssh bricksac@serverenigma.com "cd public_html && tar -xzvf ~/deploy.tar.gz && rm ~/deploy.tar.gz"
```

## Datos de la Empresa

- **Razón Social:** BRICK Proyectos & Construcción S.A.C.
- **RUC:** 20505099584
- **Inicio Actividades:** 18/09/2002
- **Dirección:** Av. Benavides Nro. 4883 Int. 701, Santiago de Surco, Lima
- **Teléfonos:** 942 115 898 | (01) 602 6936
- **Email:** administracion@bricksac.com
- **Web:** [bricksac.com](https://bricksac.com)

---

Desarrollado por [Enigma Developers SAC](https://enigmasac.com)
