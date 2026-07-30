# Identidad de Marca — Fenalco Santander

Micrositio estático con el manual de identidad visual, logotipos descargables y paleta de marca de Fenalco. Sin backend, sin base de datos — contenido público institucional.

## Estructura

```
identidad-fenalco/
├── index.html                  ← página única, todo el sitio
└── assets/
    ├── logos/                  ← 6 versiones de logo en PNG (positivo/negativo, transparente)
    ├── logos-fenalco.zip       ← pack completo para descarga en 1 clic
    └── manual/
        └── Manual_Identidad_Fenalco.pdf
```

## Deploy en Render (Static Site) — 5 minutos

1. Sube esta carpeta a un repo nuevo en `comunicaciones2-star` (ej. `fenalco-identidad-marca`).
2. En Render: **New → Static Site**.
3. Conecta el repo. Configuración:
   - **Build Command:** (dejar vacío)
   - **Publish Directory:** `.` (raíz)
4. Deploy. Render entrega una URL tipo `fenalco-identidad-marca.onrender.com`.
5. Opcional: apuntar un subdominio propio (ej. `marca.fenalcosantander.com`) desde el proveedor DNS institucional hacia el dominio de Render.

No requiere variables de entorno, base de datos ni proceso de build — es HTML/CSS/JS puro servido como archivos estáticos.

## Pendientes antes de compartir el link con afiliados/otras áreas

- **Vectoriales editables (.AI/.EPS/.SVG):** este sitio usa PNG de alta resolución extraídos del manual. Para piezas de producción, solicitar los archivos fuente originales a Comunicaciones y reemplazar/ampliar `assets/logos/`.
- **Descriptor seccional "SANTANDER":** el manual solo trae ejemplos de otras seccionales (Antioquia, Córdoba, etc.). Falta construir la versión oficial "Fenalco + Santander" según la retícula del manual (páginas 46-48) y agregarla al pack de descargas.
- **Fuentes con licencia (Soho Std, Soho Gothic Pro, Metropolis):** no vienen en el manual público. Si se necesitan para piezas de diseño, solicitar los archivos de fuente a Comunicaciones.

## Mantenimiento

Todo el sitio es un solo archivo (`index.html`) con CSS embebido — sin dependencias externas salvo las imágenes locales. Para actualizar colores, textos o agregar logos, editar directamente ese archivo.
