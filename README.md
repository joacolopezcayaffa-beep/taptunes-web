# TapTunes™ — Landing Page

Reproductor NFC con estética de mini tocadiscos.

## Deploy en Vercel (paso a paso)

### Opción A — Deploy directo desde carpeta (más fácil)

1. Andá a [vercel.com](https://vercel.com) y creá una cuenta (podés usar tu email o GitHub)
2. Una vez adentro, hacé click en **"Add New" → "Project"**
3. Elegí **"Import Git Repository"** o arrastrá la carpeta del proyecto
4. Vercel detecta automáticamente que es Vite + React
5. Click en **"Deploy"**
6. En 1-2 minutos tenés tu web online en `tu-proyecto.vercel.app`

### Opción B — Vía GitHub (recomendado para actualizaciones)

1. Creá un repositorio en [github.com](https://github.com) → "New Repository" → nombre: `taptunes-web`
2. Subí todos los archivos de esta carpeta al repo
3. En Vercel, conectá tu cuenta de GitHub
4. Importá el repositorio `taptunes-web`
5. Deploy automático cada vez que subas cambios

### Correr en local (para desarrollo)

```bash
npm install
npm run dev
```

Abre http://localhost:5173

## Estructura del proyecto

```
taptunes-deploy/
├── index.html              ← HTML base con meta tags y favicon
├── package.json            ← Dependencias (React + Vite)
├── vite.config.js          ← Configuración de Vite
├── src/
│   ├── main.jsx            ← Entry point de React
│   └── TapTunesLanding.jsx ← Componente principal (toda la landing)
└── README.md
```

## Personalización

- **Textos:** Editá directamente en `TapTunesLanding.jsx`, buscá los strings en español
- **Colores:** Las variables CSS están al inicio del archivo (`:root { ... }`)
- **Precio:** Buscá `USD 89` y `USD 119` en el componente `Comprar`
- **WhatsApp:** Agregá tu link en el footer

## Próximos pasos

- Conectar botón "Reservar" al checkout de Shopify
- Agregar Google Analytics / Meta Pixel
- Configurar dominio personalizado en Vercel
