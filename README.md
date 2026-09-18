# Landing Somos Kronos

Sitio estático de una sola página. No necesita build: `index.html` + `assets/` + `support.js`.

## Ver en local

```
npx serve .
```

## Publicar en GitHub

```
git remote add origin https://github.com/TU_USUARIO/somos-kronos-web.git
git push -u origin main
```

(Crea antes el repo vacío en GitHub, sin README/licencia, para que el push no choque con nada.)

## Publicar en Netlify

1. "Add new site" → "Import an existing project" → conecta el repo de GitHub.
2. Build command: (vacío/ninguno). Publish directory: `/` (la raíz).
3. Deploy.

## Sobre el video VSL

La sección "Mira esto primero" usa un embed de YouTube (`youtube-nocookie.com/embed/7TL6ZsWHWEM`), no un archivo de video. El `.mov` original (317 MB) sigue en `assets/` en tu máquina pero está en `.gitignore` — no se sube al repo porque ya no se necesita.
