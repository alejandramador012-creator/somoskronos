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

## ⚠️ Sobre el video VSL

`assets/vsl-somos-kronos.mov` pesa 317 MB y **no está incluido en este repo** (está en `.gitignore`) porque supera el límite de 100 MB por archivo de GitHub — el push fallaría si se agrega tal cual.

Antes de publicar, elige una opción:

- **Recomendado — hospedarlo aparte:** sube el video a YouTube (no listado) o Vimeo y avísame el link; cambio el reproductor de `index.html` por ese embed. Carga más rápido, funciona mejor en móvil y no depende del tamaño del repo.
- **Alternativa — mantenerlo auto-alojado:** usar Git LFS (`git lfs track "*.mov"`) para subirlo igual. Ten en cuenta que GitHub LFS gratis da 1 GB de almacenamiento y 1 GB de transferencia al mes — con un solo video de 317 MB el ancho de banda se agota rápido, y Netlify necesita configuración extra (Large Media / build plugin) para servirlo bien.

Sin resolver esto, el sitio publicado mostrará la sección VSL sin video.
