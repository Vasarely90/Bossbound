# Bossbound website - Netlify fixed

Deze versie is geschikt voor GitHub + Netlify.

## Belangrijk
De `index.html` staat in de hoofdmap. Netlify bouwt automatisch een `dist` map en publiceert die map.

## GitHub + Netlify stappen
1. Pak deze ZIP uit.
2. Upload de inhoud naar je GitHub repository. Let op: `index.html`, `package.json` en `netlify.toml` moeten direct in de hoofdmap van je repository staan.
3. Ga in Netlify naar **Site configuration** > **Build & deploy**.
4. Zet:
   - Build command: `npm run build`
   - Publish directory: `dist`
5. Klik op **Trigger deploy** > **Deploy site**.

## Krijg je nog 404?
Controleer dan of je niet per ongeluk de map `bossbound-netlify-fixed` als submap in GitHub hebt gezet. De bestanden moeten zo staan:

```text
/index.html
/package.json
/netlify.toml
/_redirects
/css/style.css
/js/app.js
/assets/images/...
```

Niet zo:

```text
/bossbound-netlify-fixed/index.html
```
