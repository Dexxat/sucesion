# DAMO, DOMINGO ERNESTO — Dossier de Pruebas
## Expte. 26712-2019 | Sucesión Testamentaria

Sitio estático de documentación y pruebas para uso en el proceso sucesorio.

---

### Estructura del proyecto

```
dossier-damo/
├── index.html     # Página principal (mapa, personas, cronología, delitos, comentario)
├── mapa.html      # Mapa societario interactivo (standalone)
├── assets.js      # Archivos embebidos en base64 (imágenes y PDFs)
└── _headers       # Headers de seguridad para Cloudflare Pages
```

---

### Deploy en Cloudflare Pages

1. Subir este repositorio a GitHub (repo privado recomendado)
2. Ir a [Cloudflare Pages](https://pages.cloudflare.com/)
3. **Create a project** → **Connect to Git** → seleccionar el repo
4. Configuración de build:
   - **Framework preset:** `None`
   - **Build command:** *(dejar vacío)*
   - **Build output directory:** `/` *(raíz del repo)*
5. Click **Save and Deploy**

El sitio queda en `https://[nombre-proyecto].pages.dev`

---

### Deploy en GitHub Pages (alternativa)

1. En el repo → **Settings** → **Pages**
2. Source: **Deploy from a branch** → `main` → `/ (root)`
3. El sitio queda en `https://[usuario].github.io/[repo]`

---

### Notas de seguridad

- Se recomienda repo **privado** en GitHub
- Para acceso restringido usar **Cloudflare Access** (gratis en el free tier)
- Los archivos en `assets.js` contienen los documentos embebidos en base64

---

*Todas las pruebas son de carácter público o de uso interno del proceso sucesorio.*
