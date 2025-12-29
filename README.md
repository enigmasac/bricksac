# BRICK Proyectos & Construcción S.A.C.

Landing page corporativa para BRICK, empresa peruana de ingeniería, arquitectura y construcción con más de 24 años de trayectoria.

## Stack Técnico

- **HTML5** semántico
- **Tailwind CSS** (CDN)
- **Alpine.js** para interactividad
- **Font Awesome** iconos
- **Google Fonts** (Inter)

## Estructura

```
├── index.html          # Single page principal
└── assets/
    ├── logo.png
    ├── logo-v2.png
    ├── logo-v3.png
    ├── hero-video.mp4  # Video de fondo hero
    └── projects/       # Imágenes del portafolio
        ├── bbva-comedor.jpg
        ├── bbva-becs.jpg
        ├── bbva-sotano.jpg
        ├── centenario-oficinas.jpg
        └── pluz-energia.jpg
```

## Secciones

1. **Hero** - Video de fondo con CTA
2. **Estadísticas** - Años, proyectos, m² construidos
3. **Nosotros** - Misión, visión y valores
4. **Servicios** - Diseño, construcción, instalaciones
5. **Proyectos** - Portafolio con filtros
6. **Certificaciones** - SGS, HODELPE, Pacto Mundial, ESR
7. **Contacto** - Formulario y datos de contacto
8. **Footer** - Links y créditos

## Deploy

El sitio se despliega en el servidor de Enigma:

```bash
ssh bricksac@serverenigma.com
# Destino: ~/public_html/
```

## Datos de la Empresa

- **Razón Social:** BRICK Proyectos & Construcción S.A.C.
- **RUC:** 20505099584
- **Inicio Actividades:** 18/09/2002
- **Dirección:** Av. Benavides Nro. 4883 Int. 701, Santiago de Surco, Lima
- **Teléfonos:** 942 115 898 | (01) 602 6936
- **Email:** administracion@bricksac.com
- **Web:** [bricksac.com](https://bricksac.com)

## Desarrollo

```bash
# Servidor local
python3 -m http.server 8080

# Abrir en navegador
open http://localhost:8080
```

---

Desarrollado por [Enigma Developers SAC](https://enigmasac.com)
