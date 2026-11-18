# Publicar y actualizar LYCAN (GitHub Pages)

## Archivos (todos en la raíz del repositorio de la app)
`index.html` · `manifest.json` · `sw.js` · `icon-192.png` · `icon-512.png` · `icon-maskable-512.png`

## Primera vez
1. Crea un repositorio **público** (por ejemplo `lycan-app`), distinto del privado de copias.
2. **Add file → Upload files**: sube los 6 archivos y **Commit changes**.
3. **Settings → Pages → Deploy from a branch → main / (root) → Save**.
4. En 1–2 minutos abre `https://TU-USUARIO.github.io/lycan-app/` en el teléfono.
5. Instálala: Chrome/Android → botón **📲 Instalar** (pestaña Más) o menú ⋮ → *Instalar app*; Safari/iPhone → Compartir → *Añadir a pantalla de inicio*.

## Cada versión nueva (v44 incluida)
1. Sube **`index.html`** y **`sw.js`** (reemplazan a los anteriores). Si hay íconos nuevos, súbelos también.
2. Cierra la app por completo y ábrela de nuevo. Si ves el aviso «Hay una versión nueva», toca **Actualizar**.
3. Para que aparezca ese aviso en futuras versiones, cambia el número en `sw.js` (`lycan-v45` → `lycan-v45`).
4. Actualiza con los bots detenidos. Tus datos se conservan; si falta algo, ☁️ **Respaldo en la nube → Versiones anteriores**.

## Avisos al celular y segundo plano (desde v44)
- **Instala la app** y permite las notificaciones: en Android los avisos solo funcionan con la app instalada o desde la dirección https.
- En **Más → 🔔 Avisos y segundo plano** eliges qué avisos recibir (resultado de operaciones, inicio/fin del horario, aviso antes de que empiece, conexión, metas y límites).
- **Modo segundo plano** (audio inaudible + notificación «LYCAN activo») ayuda a que el sistema no pause la app al cambiar de aplicación o ir al inicio. Puede pausar tu música.
- **Recordar token** (opcional, cifrado en este dispositivo) permite que la app se reconecte sola si el sistema la cierra.
- Límite real: una página web no puede operar con la app cerrada o el teléfono bloqueado mucho tiempo, ni enviar avisos si no está abierta. Para eso haría falta un servidor.

## Importante
- El repositorio de la app es público: **nunca pongas tokens ni datos personales dentro**. El token solo se escribe en la app.
- El nombre del repositorio de copias viene precargado en el código; déjalo en blanco antes de publicar si no quieres que sea visible.
- Google Drive solo funciona desde una dirección https como esta.
