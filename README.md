# BRICK Proyectos & Construcción S.A.C.

Landing page corporativa para BRICK, empresa peruana de ingeniería, arquitectura y construcción con más de 24 años de trayectoria.

## Stack Técnico

- **HTML5** semántico
- **Tailwind CSS** (CDN) + config modular
- **Alpine.js** para interactividad (lightbox/carousel)
- **Font Awesome** iconos
- **Google Fonts** (Inter)

## Estructura

```
web/
├── index.html              # Single page principal
├── css/
│   └── styles.css          # Estilos personalizados
├── js/
│   └── tailwind.config.js  # Config de Tailwind
└── assets/
    ├── logos/              # Logos de la empresa
    │   ├── logo.png
    │   ├── logo-v2.png
    │   └── logo-v3.png
    ├── media/              # NO en git
    │   └── hero-video.mp4
    ├── projects/           # NO en git
    │   └── *.jpg, *.png
    └── certifications/     # NO en git
        └── logo-*.png, logo-*.jpg
```

## Archivos excluidos de Git

El `.gitignore` excluye multimedia pesada:
- `assets/media/` (video hero ~11MB)
- `assets/projects/` (fotos de proyectos)
- `assets/certifications/` (logos de certificaciones)

Estos archivos se mantienen solo en el servidor y en local.

## Deploy

```bash
# 1. Comprimir (sin multimedia pesada)
tar -czvf deploy.tar.gz --exclude='.git' --exclude='assets/media/hero-video.mp4' .

# 2. Subir al servidor
scp deploy.tar.gz bricksac@serverenigma.com:~/

# 3. Descomprimir en servidor (usar usuario debian para permisos)
ssh debian_enim "cd /home/bricksac/public_html && sudo tar -xzvf /home/bricksac/deploy.tar.gz && sudo chown -R bricksac:bricksac . && sudo rm /home/bricksac/deploy.tar.gz"
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
