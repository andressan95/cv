# Sitio web — Cristóbal Andrés Sánchez Cobeña

Hoja de vida personal (una sola página, bilingüe ES/EN). Sitio estático autocontenido.

## Publicar en Vercel

### Opción A — Subir la carpeta (sin GitHub)
1. Entra a https://vercel.com → **Add New → Project → Deploy**.
2. Arrastra esta carpeta (o su contenido). Vercel detecta `index.html` y lo publica.
3. **Settings → Domains** → agrega `ideass.me`.

### Opción B — Con GitHub (recomendado)
Desde una terminal, dentro de esta carpeta:

```bash
git init
git add .
git commit -m "Sitio web ideass.me"
git branch -M main
git remote add origin https://github.com/andressan95/ideass-web.git
git push -u origin main
```

> Primero crea el repositorio vacío en https://github.com/new (por ejemplo `ideass-web`).

Luego en Vercel: **Add New → Project → Import** ese repo. Cada `git push` vuelve a desplegar.

## Archivos
- `index.html` — el sitio completo (fotos, fuentes y estilos incrustados).
- `vercel.json` — configuración de despliegue.
