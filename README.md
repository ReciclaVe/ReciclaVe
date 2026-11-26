# Sistema Inteligente de Gestión y Valorización de Residuos – Gran Caracas

Proyecto postulado a **Innova Ciudad** (ciudades inteligentes) de la plataforma Innova Venezuela. Propone contenedores inteligentes con sensores IoT, una planta que separa y compacta por material, una plataforma de trazabilidad y un sistema de tokens por peso verificado, con inclusión de comunas y recolectores. Zona piloto: San Antonio de los Altos (4 sectores, 16 puntos).

> **Estado:** diseño y simulación. No hay mediciones del sensor, del pesaje ni de la compactadora. Las cifras económicas y de impacto son estimaciones del equipo.

## Contenido

| Carpeta | Qué contiene |
| --- | --- |
| `index.html` | Aplicación web de demostración (HTML, CSS y JavaScript en un solo archivo): mapa de los 16 puntos, ruta de recolección, ruta al contenedor más cercano, escaneo de QR, entrega con fotos, tokens y canje. |
| `docs/` | Ficha técnica (Word), documento del proyecto (PDF) y presupuesto de prototipos (PDF). |
| `docs/imagenes/` | Esquema del contenedor inteligente y esquema conceptual de la compactadora. |
| `docs/fuentes/` | Anteproyecto y resumen de diapositivas originales. |

## Ver la demo

- **Local:** abre `demo/index.html` en un navegador con conexión a internet (usa Leaflet, mosaicos de mapa y OSRM).
- **GitHub Pages (recomendado para presentar):** en el repositorio, *Settings → Pages → Deploy from a branch → main / (root)*; la demo quedará en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/demo/`. Con HTTPS, la cámara y la ubicación funcionan con menos restricciones que al abrir el archivo desde el disco.

## Limitaciones de la demo

- Los datos (llenado, saldos, historial) son simulados y se guardan en `localStorage` del navegador; no se comparten entre dispositivos.
- El selector de rol no tiene autenticación. El QR contiene la cédula en texto plano, sin firma. No es apto para uso real.
- Las fotos de evidencia no se suben ni se guardan.
- Algunas coordenadas de los puntos son aproximadas o provienen de Plus Codes por confirmar.
- Depende de servicios externos: Leaflet, mosaicos de mapa, OSRM (servidor de demostración) y librerías de QR.

## Pendientes

- Coordenadas verificadas de los 16 puntos y ubicación de la planta.
- Mediciones del sensor, del pesaje y de la compactadora; fuente de presión del Prototipo B.
- Presupuesto con cotizaciones, cartas de aval y datos del municipio.
- Carreras, tutor e integrantes en la ficha técnica.
- Licencia del repositorio (por definir por el equipo).
