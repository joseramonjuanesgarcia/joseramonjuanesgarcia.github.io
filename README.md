# Web personal (Quarto)

Sitio web académico personal. Hecho con [Quarto](https://quarto.org).

## Estructura

| Archivo | Qué es |
|---|---|
| `_quarto.yml` | Configuración del sitio (título, menú, enlaces, tema). |
| `index.qmd` | Página de inicio (foto + bio + enlaces). |
| `research.qmd` | Papers y working papers. |
| `cv.qmd` | CV (enlaza `cv.pdf`, que debes añadir). |
| `teaching.qmd` | Docencia. |
| `styles.scss` | Colores y tipografía. |
| `profile.svg` | Foto de perfil provisional — **sustitúyela por la tuya**. |

Busca los comentarios `<-- EDITA` para saber qué cambiar.

## Editar y previsualizar en local

Requiere tener Quarto instalado (`brew install --cask quarto`).

```bash
quarto preview     # abre el sitio en el navegador y se recarga al guardar
```

## Publicar en GitHub Pages

```bash
git init && git add . && git commit -m "Web personal"
# crea el repo TUUSUARIO.github.io en GitHub y luego:
git remote add origin https://github.com/TUUSUARIO/TUUSUARIO.github.io.git
git push -u origin main
quarto publish gh-pages
```

Tu web quedará en `https://TUUSUARIO.github.io`.

## Tu foto

Guarda tu foto como `profile.jpg` (o `.png`) en esta carpeta y cambia
`image: profile.svg` por `image: profile.jpg` en `index.qmd`.
