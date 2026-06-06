# Ventas Distritodo — App instalable (PWA)

Dashboard de cumplimiento de metas, proyección y pipeline de ventas para asesores
y puntos de venta. Se instala en celular y computadora como una app, con ícono propio.

---

## Qué necesitas (una sola vez)

1. **Node.js** instalado en tu computadora. Descárgalo en https://nodejs.org (versión LTS).
   Para comprobar que quedó instalado, abre una terminal y escribe: `node -v`
2. Una cuenta gratuita en **Vercel** (https://vercel.com) — puedes entrar con tu cuenta de Google.

---

## Paso 1 — Probar la app en tu computadora

Abre una terminal dentro de la carpeta del proyecto y ejecuta:

```bash
npm install
npm run dev
```

Te mostrará una dirección como `http://localhost:5173`. Ábrela en el navegador
y verás el dashboard funcionando. Para detenerlo, presiona Ctrl + C.

---

## Paso 2 — Publicarlo en internet (gratis con Vercel)

Esta es la forma más sencilla, sin usar comandos:

1. Entra a https://vercel.com e inicia sesión.
2. Crea una cuenta gratuita en https://github.com si no tienes, y sube esta carpeta
   a un repositorio nuevo (botón "Add file" → "Upload files" en GitHub, arrastra todo
   MENOS la carpeta `node_modules`).
3. En Vercel: "Add New" → "Project" → elige el repositorio que acabas de subir.
4. Vercel detecta Vite automáticamente. Solo presiona **Deploy**.
5. En menos de un minuto te da un enlace público, por ejemplo:
   `https://ventas-distritodo.vercel.app`

Ese enlace es tu app. Compártelo con tu equipo.

### Alternativa por terminal (más rápida si ya usas Node)

```bash
npm install -g vercel
vercel
```

Sigue las preguntas (acepta los valores por defecto) y al final te dará el enlace.

---

## Paso 3 — "Instalar" la app en cada dispositivo

Una vez tengas el enlace público, ábrelo en el navegador del celular o computadora:

- **Android (Chrome):** menú ⋮ → "Agregar a pantalla de inicio" / "Instalar app".
- **iPhone (Safari):** botón compartir ⬆️ → "Agregar a pantalla de inicio".
- **Computadora (Chrome/Edge):** aparece un ícono de instalar ⊕ en la barra de
  direcciones, o menú ⋮ → "Instalar Ventas Distritodo".

Queda con su ícono propio y se abre como una aplicación, sin barra de navegador.

---

## Uso

- Botón **Cargar Excel**: sube la plantilla (`plantilla-asesores.xlsx`) con las hojas
  "Asesores" y "Puntos de Venta". La app actualiza ambas secciones.
- También puedes editar cada registro con el ícono ✎ o agregar/eliminar manualmente.

Nota: los datos se cargan desde el Excel cada vez que abres la app; no se guardan
de forma permanente.
