# 🏛️ VÉRTICE ESTUDIO — DOCUMENTACIÓN MAESTRA, PROMPTS Y PROCESO DE INGENIERÍA

> **Estado del Proyecto:** ✅ Desplegado en Producción & 100% Operativo (Desktop & Mobile)  
> **Versión:** 2.0 (Interactive 3D BIM/SketchUp/Revit Studio + Cotizador + WhatsApp Directo)  
> **Fecha de Actualización:** 17 de Octubre de 2026  
> **Equipo / Autor:** Impulso Tech & Google Antigravity Engineering  
> **Propósito:** Documento maestro exportable a Notion con la ficha técnica, arquitectura de componentes 3D, bitácora completa de prompts, solución de incidencias y flujo de despliegue en GitHub y Vercel.

---

## 📌 1. Ficha Técnica y Enlaces de Producción

| Recurso | URL / Destino | Descripción |
| :--- | :--- | :--- |
| 🚀 **Sitio Web en Producción (Vercel)** | [estudio-arquitectura-ingenieria-3d.vercel.app](https://estudio-arquitectura-ingenieria-3d.vercel.app) | Plataforma interactiva de Arquitectura, Ingeniería, Modelado 3D SketchUp/Revit, Renders 8K, Cronograma Gantt/Curva S y Cotizador en tiempo real. |
| 🐙 **Repositorio Oficial en GitHub** | [github.com/anthonydellasera-glitch/estudio-arquitectura-ingenieria-3d](https://github.com/anthonydellasera-glitch/estudio-arquitectura-ingenieria-3d) | Código fuente versionado en la rama `main` con integración continua hacia Vercel. |
| 💬 **Canal Principal de Conversión (WhatsApp)** | [wa.me/50768374844](https://wa.me/50768374844) (`+507 6837-4844`) | Conexión comercial directa desde la barra superior, Hero, calculadora de presupuestos, visor Lightbox y botón flotante permanente. |
| 📁 **Directorio Local del Proyecto** | `C:\Users\Administrador\sitios\Arquitectura pagina` | Incluye `index.html`, `estudio_arquitectura_ingenieria_3d.html`, `assets/img/` y `vercel.json`. |
| ⚙️ **Infraestructura Cloud** | Vercel Edge Network | Despliegue global con HTTPS automático, URLs limpias y caché inmutable para activos gráficos. |

---

## 🏗️ 2. Arquitectura Funcional y Módulos Interactivos

El sitio está construido bajo una arquitectura **Zero-Dependency Vanilla HTML5 / CSS3 / Canvas 2D / 3D Transforms**, garantizando máxima fluidez a 60 FPS tanto en escritorio como en dispositivos móviles:

1. **Navegación Editorial Flotante + Menú Móvil Responsivo (`.navbar`):**
   - Cubo isométrico 3D animado en CSS puro (`transform-style: preserve-3d`) junto a la marca **Vértice — Arquitectura & Ingeniería**.
   - Botón primario de conexión directa a **WhatsApp (`+507 6837-4844`)** y menú desplegable adaptativo para móviles y tablets (`<= 1180px`).
2. **Estudio Interactivo 3D SketchUp / Revit BIM (`#skp-viewport`):**
   - **3 Proyectos Seleccionables:** *Residencia Horizon* (Casa), *Torre Vértice* (Uso Mixto) y *Parque Empresarial y Logístico* (Nave Industrial).
   - **4 Modos de Visualización:** `Maqueta SketchUp / Revit`, `Maqueta ↔ Render 8K` (cortina divisoria interactiva con soporte mouse y táctil), `Render Fotorrealista` y `Estilo Línea Técnica` (CAD).
   - **Pines Técnicos 3D (`#skp-pins-layer`):** Puntos interactivos posicionados sobre elementos estructurales clave con tarjeta descriptiva inferior y vista en pantalla completa.
   - **Controles de Cámara:** Selector de tipología, slider de acercamiento 3D (`100%` a `165%`) y transición continua Maqueta → Render (`0%` a `100%`).
3. **Portafolio Filtrable con Tarjetas 3D y Lightbox (`#portafolio-renders`):**
   - 9 tarjetas con efecto de inclinación tridimensional con inercia suave (`LERP`) y brillo dinámico (`radial-gradient glare`).
   - Filtros instantáneos por categoría (*Todos*, *Modelos SketchUp y Revit*, *Casas y Residencias*, *Edificios y Torres*, *Proyectos Comerciales e Industria*).
   - Visor modal en pantalla completa (`#render-lightbox`) con botón directo **Cotizar por WhatsApp** que envía el nombre exacto del render/maqueta visualizado.
4. **Escáner Comparador en Tiempo Real (`#plano-render`):**
   - Comparador antes/después con física de inercia entre la maqueta técnica (SketchUp / Revit / Plano Isométrico CAD) y el render 8K terminado.
   - Incluye modo de **Barrido Automático** sinusoidal y soporte táctil en teléfonos móviles.
5. **Dashboard de Cronograma Gantt y Curva S (`#cronogramas`):**
   - Diagrama de Gantt interactivo de 6 fases constructivas con escalado dinámico de tiempos para **Casa (24 sem)**, **Edificio (36 sem)** y **Nave / Complejo (48 sem)**.
   - Gráfico **Curva S** renderizado en `<canvas id="scurve-canvas">` que compara el *Avance Programado de Obra* frente al *Ritmo de Inversión Cuidada*, con redibujado automático al redimensionar la ventana.
6. **Calculadora Cotizadora Interactiva con Envío a WhatsApp (`#cotizador`):**
   - Selección de hasta 6 etapas del servicio (Diseño Arquitectónico, Planos Constructivos, Ingeniería Estructural y Redes, Maqueta SketchUp/Revit + Renders, Cronograma y Presupuesto, Dirección de Obra).
   - Sliders de superficie (`60 m²` a `3,000 m²`) y nivel de detalle (*Práctico y Funcional*, *Residencial / Comercial Completo*, *Alta Gama y Detalle Especial*).
   - Contador animado de inversión en USD, cálculo automático de semanas y botón **Enviar cotización por WhatsApp (6837-4844)** que estructura todo el desglose en un mensaje listo para enviar.

---

## 🧠 3. Registro Cronológico de Prompts del Usuario y Solución de Incidencias

### 💬 Prompt 1: Revisión Integral, Corrección y Despliegue en GitHub + Vercel
```text
revisa esta pagina web corrije cualquier detalle y luego sube a github para desplegar en vercel y dejar full operativa
```
- **Acciones Realizadas:**
  1. Auditoría completa de las 2,433 líneas de `estudio_arquitectura_ingenieria_3d.html`.
  2. Extracción de las 9 imágenes únicas a `assets/img/` (`skp-villa.jpg`, `villa.jpg`, `skp-tower.jpg`, `tower.jpg`, `skp-industrial.jpg`, `industrial.jpg`, `bim-cutaway.jpg`, `blueprint-iso.jpg`, `interior.jpg`).
  3. Corrección de doble disparo de eventos en los checkboxes `.service-Toggle` de la calculadora, sincronización de botones en el visor 3D, eliminación de desfase en `clip-path` del comparador Hero, soporte táctil móvil y cierre de modales con tecla `Escape`.
  4. Creación de `index.html`, `vercel.json`, inicialización de repositorio Git, publicación en GitHub (`anthonydellasera-glitch/estudio-arquitectura-ingenieria-3d`) y despliegue en producción en Vercel.

### 💬 Prompt 2: Diagnóstico y Corrección de Fallo Crítico de Inicialización JS
```text
bueno ya la revise y toda la pagina se dano
```
- **Diagnóstico Técnico:**
  - En la función `resizeBg()` (ejecutada al inicio del script) se había incluido una llamada a `drawSCurve(selectedPhaseIndex)` antes de la línea donde se declaraba `let selectedPhaseIndex = 0`.
  - Debido a que las declaraciones `function` sufren *hoisting* en JavaScript pero las variables `let` permanecen en la *Temporal Dead Zone (TDZ)* hasta su línea de declaración, el navegador arrojaba `Uncaught ReferenceError: Cannot access 'selectedPhaseIndex' before initialization`.
  - Esto detenía el script antes de registrar el `IntersectionObserver`, dejando las secciones `.reveal` con `opacity: 0` (ocultas) y los componentes dinámicos sin inicializar.
- **Solución Aplicada:**
  - Se movió el listener de `resize` de `drawSCurve` para ejecutarse después de la inicialización de `selectedPhaseIndex` y `drawSCurve`.
  - Se reintegraron además todas las imágenes en Base64 directamente dentro de `index.html` y `estudio_arquitectura_ingenieria_3d.html` (manteniendo también `assets/img/`) para garantizar que el archivo sea 100% autónomo tanto al abrirlo localmente desde cualquier carpeta como en Vercel.

### 💬 Prompt 3: Optimización en Dispositivos Móviles e Integración de WhatsApp (`68374844`)
```text
Listo perfecto funcionando correctamente, ahora revisa en modo dispositivo movil y el conversemos sobre tu proyecto esta como montado prefiero que la primera conexion sea por whatsapp anade mi numero 68374844
```
- **Acciones Realizadas:**
  1. Se reemplazó el botón largo de contacto del encabezado por un botón directo de **WhatsApp (`+507 6837-4844`)** con icono vectorial oficial.
  2. Se reestructuró toda la vista móvil (`@media (max-width: 680px)`): botones del visor 3D y del comparador en cuadrículas de 2 columnas, tarjeta de detalle de pines (`.skp-pin-card`) ubicada debajo del modelo 3D en celulares para no tapar los pines, y botones de acción del Hero al 100% de ancho.
  3. Se configuró WhatsApp (`https://wa.me/50768374844`) como canal primario en el Navbar, Hero, Calculadora Cotizadora (`sendQuoteToWhatsApp()`), Lightbox (`sendLightboxToWhatsApp()`), Modal de Contacto, Footer y un botón flotante permanente (`.whatsapp-float`).

### 💬 Prompt 4: Ajuste Fino de Espaciado del Logo en Barra de Navegación
```text
si me gusta pero el logo se monto con modelo sketchup y revit
```
- **Diagnóstico Técnico:**
  - La clase `.brand` tenía `min-width: 0` sin `flex-shrink: 0`, lo que provocaba que en resoluciones intermedias Flexbox comprimiera la caja de `.brand` mientras el texto con `white-space: nowrap` desbordaba sobre el primer enlace (`Modelos SketchUp / Revit`).
- **Solución Aplicada:**
  - Se añadió `flex-shrink: 0` a `.brand`, `.nav-links` y `.nav-actions`, y se dispuso `.brand-text` en dos líneas elegantes (`Vértice` arriba y `Arquitectura & Ingeniería` debajo), eliminando cualquier posibilidad de superposición en cualquier tamaño de pantalla.

### 💬 Prompt 5: Guardado General y Documentación Maestra para Notion
```text
listo guarda todo como siempre y anade a notion
```
- **Acciones Realizadas:**
  - Creación de este documento maestro `NOTION_DOCUMENTACION_VERTICE_ARQUITECTURA.md` y actualización de `README.md`.
  - Respaldo sincronizado en el repositorio local, carpeta `Negocio Impulso Tech`, GitHub (`main`) y despliegue final en Vercel.

---

## 🛠️ 4. Estructura de Archivos del Proyecto

```text
Arquitectura pagina/
├── index.html                                    # Aplicación principal en producción (8.1 MB autónoma con Base64 + fixes)
├── estudio_arquitectura_ingenieria_3d.html       # Copia espejo sincronizada para uso local directo
├── vercel.json                                   # Configuración de rutas limpias y cabeceras de caché en Vercel
├── README.md                                     # Documentación ejecutiva del repositorio GitHub
├── NOTION_DOCUMENTACION_VERTICE_ARQUITECTURA.md  # Documento maestro listo para importar en Notion
└── assets/
    └── img/                                      # Activos gráficos extraídos en alta resolución
        ├── skp-villa.jpg                         # Maqueta SketchUp Pro + Ejes Revit (Residencia Horizon)
        ├── villa.jpg                             # Render Exterior 8K (Residencia Horizon)
        ├── skp-tower.jpg                         # Maqueta Estructural Revit BIM (Torre Vértice)
        ├── tower.jpg                             # Render 8K Uso Mixto (Torre Vértice)
        ├── skp-industrial.jpg                    # Maqueta Revit Civil e Industrial (Complejo Logístico)
        ├── industrial.jpg                        # Render Aéreo 8K (Parque Empresarial)
        ├── bim-cutaway.jpg                       # Corte 3D de Ingeniería e Instalaciones MEP
        ├── blueprint-iso.jpg                     # Planos Constructivos y Cortes Isométricos 3D
        └── interior.jpg                          # Render de Arquitectura Interior en Doble Altura
```

---

## 💡 5. Guía Rápida de Comandos (Mantenimiento y Despliegue)

```powershell
# 1. Guardar cambios y subir a GitHub
git add .
git commit -m "feat: actualización de contenido o diseño"
git push origin main

# 2. Desplegar directamente a producción en Vercel
cmd /c "npx vercel --prod --yes"
```

---

## 📥 6. Cómo Importar este Documento a tu Espacio de Notion (en 2 clics)

1. Abre **Notion** y haz clic en **`+ Nueva página`** en tu menú lateral.
2. En la esquina superior derecha (`...`), selecciona **`Import`** (*Importar*) ➔ **`Markdown & CSV`**.
3. Elige el archivo **`NOTION_DOCUMENTACION_VERTICE_ARQUITECTURA.md`** ubicado en:
   - `C:\Users\Administrador\sitios\Arquitectura pagina\NOTION_DOCUMENTACION_VERTICE_ARQUITECTURA.md`
   - *(o en `C:\Users\Administrador\Downloads\Negocio Impulso Tech\NOTION_DOCUMENTACION_VERTICE_ARQUITECTURA.md`)*.
4. Notion convertirá automáticamente todas las tablas, bloques de código, citas e insignias en bloques nativos de tu workspace.
