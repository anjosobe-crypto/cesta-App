# CestaApp 🛒

App PWA (Progressive Web App) para gestionar la cesta de la compra, instalable en Android.

## 📱 Cómo instalar en Android

### Opción 1 — Servir localmente en tu red WiFi
1. Necesitas un ordenador en la misma red WiFi que el móvil
2. Instala Node.js si no lo tienes: https://nodejs.org
3. En la carpeta de la app, ejecuta:
   ```
   npx serve -l 8080
   ```
4. En tu Android, abre Chrome y ve a: `http://[IP-de-tu-ordenador]:8080`
5. Aparecerá un banner "Añadir a pantalla de inicio" → pulsa Instalar

### Opción 2 — Subir a hosting gratuito (recomendado)
Sube los 3 archivos a cualquiera de estos servicios gratuitos:
- **Netlify Drop**: ve a https://app.netlify.com/drop y arrastra la carpeta
- **GitHub Pages**: sube a un repositorio público y activa Pages
- **Vercel**: https://vercel.com (conecta tu GitHub)

Una vez publicada con HTTPS, en Chrome Android aparecerá automáticamente el banner de instalación.

### Opción 3 — Usar GitHub Pages paso a paso
1. Crea cuenta en https://github.com
2. Nuevo repositorio → súbele los 3 archivos (index.html, manifest.json, sw.js)
3. Settings → Pages → Source: main branch → Save
4. Tu app estará en: `https://TU-USUARIO.github.io/NOMBRE-REPO`
5. Abre esa URL en Chrome Android → menú (⋮) → "Añadir a pantalla de inicio"

## 🔧 Funcionalidades

- ✅ Gestión completa de productos con todos los campos
- 📊 Análisis de gasto por categoría, evolución y supermercados  
- 📈 Histórico de precios con gráficas
- 🏪 Comparativa de precios entre supermercados
- 💰 Presupuesto mensual con alertas visuales
- 📝 Lista automática de compra basada en hábitos
- 📷 Escaneo de tickets con OCR (Tesseract.js)
- 🔔 Recordatorios de productos habituales
- 🔮 Predicción de gasto mensual
- 🕐 Detección de mejores momentos para comprar

## 📁 Archivos
- `index.html` — App completa
- `manifest.json` — Configuración PWA para instalación
- `sw.js` — Service Worker (funcionamiento offline)

## 💡 Notas
- Todos los datos se guardan en el localStorage del navegador (privado, en tu dispositivo)
- Funciona offline una vez instalada
- Para el OCR necesitas conexión a internet la primera vez (carga Tesseract.js)
