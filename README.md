# 🇮🇹 Italiano A1–A2 App

App para aprender italiano con Speaking, Writing, Listening y Reading. Powered by Claude AI.

---

## 🚀 Cómo publicarla (paso a paso, sin experiencia técnica)

### Paso 1 — Creá una cuenta en GitHub
1. Andá a [github.com](https://github.com) y creá una cuenta gratuita
2. Hacé clic en **New repository** (botón verde)
3. Nombre: `italiano-app`
4. Dejalo en **Public**
5. Hacé clic en **Create repository**

### Paso 2 — Subí los archivos
En la página del repositorio vacío, hacé clic en **uploading an existing file** y subí:
- `server.js`
- `package.json`
- La carpeta `public/` con el archivo `index.html` dentro

Hacé clic en **Commit changes**.

### Paso 3 — Creá una cuenta en Render
1. Andá a [render.com](https://render.com) y creá una cuenta gratuita (podés entrar con GitHub)
2. Hacé clic en **New +** → **Web Service**
3. Conectá tu repositorio `italiano-app`
4. Configurá así:
   - **Name**: italiano-app (o lo que quieras)
   - **Runtime**: Node
   - **Build Command**: `npm install`
   - **Start Command**: `node server.js`
5. Hacé clic en **Create Web Service**

### Paso 4 — Agregá tu API key de Anthropic
1. En Render, andá a tu servicio → **Environment**
2. Hacé clic en **Add Environment Variable**
3. Key: `ANTHROPIC_API_KEY`
4. Value: tu API key de Anthropic (la conseguís en [console.anthropic.com](https://console.anthropic.com))
5. Guardá y Render reiniciará el servidor automáticamente

### Paso 5 — ¡Listo! 🎉
Render te da una URL del tipo `https://italiano-app-xxxx.onrender.com`.  
Esa es tu app, disponible para cualquiera con el link.

---

## 📁 Estructura del proyecto

```
italiano-app/
├── server.js        ← Servidor que protege tu API key
├── package.json     ← Dependencias
└── public/
    └── index.html   ← La app completa
```

## 💡 Notas

- El plan gratuito de Render "duerme" el servidor después de 15 min sin uso, y tarda ~30 seg en volver a despertar. Para uso personal está bien.
- Si querés que siempre esté activa, el plan de pago de Render cuesta ~$7/mes.
- La API key de Anthropic tiene costo por uso (muy bajo para estudio personal).
