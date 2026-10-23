# LionT Shop (static)

Landing / tienda estática de productos digitales **LionT** (Tito Tapias).

- **Pack FOMO** €5 → Stripe Payment Link  
- **Brief Fed** €9 → Stripe Payment Link  

Solo frontend: `index.html` + `styles.css`. Sin backend.

## Vista previa local

```bash
cd /workspace/liont-shop
python3 -m http.server 8080
# abrir http://127.0.0.1:8080/
```

O abre `index.html` directamente en el navegador.

## GitHub Pages (elegido por Tito)

Estructura lista en la **raíz del repo** (no hace falta carpeta `docs/`).

1. Crear un repo público vacío (ej. `liont-shop`) en la cuenta de Tito.
2. Autenticar `gh` o conectar GitHub en Cursor.
3. Desde esta carpeta:

```bash
cd /workspace/liont-shop
git init
git add index.html styles.css README.md .nojekyll
git commit -m "LionT shop: Pack FOMO + Brief Fed"
git branch -M main
gh repo create liont-shop --public --source=. --remote=origin --push
# Settings → Pages → Deploy from branch → main / (root)
```

URL típica (cuando exista): `https://<usuario>.github.io/liont-shop/`  
**No inventar URL hasta que el deploy esté live.**

Alternativas: arrastrar la carpeta a Cloudflare Pages o Netlify (mismo `index.html` en raíz).

## Buffer / CTAs

Los CTAs de Shorts y posts Buffer deben apuntar **aquí** (URL de Pages cuando esté publicada), no solo al perfil. Los botones de esta página ya van a los Payment Links de Stripe.

## Contacto

titotapias@gmail.com
