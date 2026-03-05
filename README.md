# 한국어 말 — PWA + Neural TTS (voz neuronal)

Este paquete funciona de 2 formas:

1) **Sin backend (GitHub Pages):** usa la voz del sistema (speechSynthesis) como respaldo.
2) **Con voz neuronal (recomendado):** despliega en **Netlify** y activa la Function `/api/tts`.
   - Así el botón ▶ usa TTS neuronal (OpenAI Speech API) y suena mucho más natural.

## Opción A — GitHub Pages (solo fallback)
- Sube `index.html`, `manifest.json`, `service-worker.js`, `icon-192.png`
- Funciona, pero el audio depende de las voces del iPad.

## Opción B — Netlify (voz neuronal)
1. Crea una cuenta en Netlify.
2. Importa tu repo (o arrastra la carpeta del proyecto).
3. En **Site settings → Environment variables** añade:
   - `OPENAI_API_KEY` = tu clave de OpenAI
4. Asegúrate de que la carpeta `netlify/functions/tts.js` está incluida en el deploy.
5. Publica.

Cuando exista `/api/tts`, la app lo usa automáticamente. Si falla, vuelve al fallback.

## Instalación en iPad
Safari → Compartir → Añadir a pantalla de inicio.
