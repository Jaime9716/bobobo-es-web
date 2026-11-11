# Versión web

Página para jugar a la traducción en el navegador con EmulatorJS (núcleo mGBA).

## Jugar en tu PC
1. Haz doble clic en `servir.bat` (necesita Python). Se abrirá http://localhost:8080.
2. Elige o arrastra la ROM japonesa original (o `parche/bobobo_es.gba`). También vale un `.zip`.
3. Si es la original, el parche `bobobo_es.ips` se aplica en el navegador y se comprueba el SHA-256.

No funciona abriendo `index.html` con doble clic (`file://`): necesita un servidor.
El emulador se descarga de cdn.emulatorjs.org, así que hace falta Internet.

## Publicarlo
Sube solo esta carpeta (`index.html`, `bobobo_es.ips`) a cualquier hosting estático
(GitHub Pages, Netlify, itch.io como juego HTML…). **No subas ninguna ROM**: cada
jugador carga la suya.

Si cambias el parche, actualiza `SHA_PARCHEADA` en `index.html` y vuelve a copiar `bobobo_es.ips` aquí.
