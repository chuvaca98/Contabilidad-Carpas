# Cotizador — Carpas & Eventos (PWA instalable)

Demo funcional para probar en el celular. Funciona offline y guarda los datos en el dispositivo.

## Archivos
- `index.html` — la app completa
- `manifest.webmanifest` — metadatos de la PWA (nombre, íconos, colores)
- `sw.js` — service worker (offline + instalación)
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` — íconos

## Importante: requiere HTTPS o localhost
El service worker y el botón de instalar **solo funcionan sobre HTTPS o en localhost**.
Abrir el `index.html` con doble clic (file://) NO permite instalar.

### Opción A — Probar en local (en tu PC)
```bash
cd carpas-cotizador
python3 -m http.server 8080
# abre http://localhost:8080
```

### Opción B — Publicar gratis (para que tu cliente lo instale en su celular)
Sube la carpeta a cualquiera de estos (todos dan HTTPS gratis):
- **Vercel**: `vercel` (o arrastra la carpeta en vercel.com)
- **Netlify**: arrastra la carpeta en app.netlify.com/drop
- **GitHub Pages**

## Cómo se instala en el celular
- **Android (Chrome):** aparece el botón "Instalar app" en la cabecera, o menú → "Agregar a pantalla de inicio".
- **iPhone (Safari):** botón Compartir → "Añadir a pantalla de inicio".

Queda con ícono propio y abre a pantalla completa, como app nativa.
