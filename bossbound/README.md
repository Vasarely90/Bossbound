# Bossbound website — Netlify ready

Deze versie is aangepast zodat het Bossbound-logo op de website een echte afbeelding is in plaats van gewone tekst.

## Netlify instellingen

Build command:

```bash
npm run build
```

Publish directory:

```text
dist
```

## Upload via GitHub

Zet deze bestanden direct in de hoofdmap van je repository:

```text
index.html
package.json
netlify.toml
_redirects
css/
js/
assets/
README.md
```

Daarna in Netlify: **Deploys → Trigger deploy → Clear cache and deploy site**.

## Wat is aangepast

- Header gebruikt nu `assets/images/bossbound-logo-header.png`
- Hero gebruikt nu `assets/images/bossbound-logo-full.png`
- Footer gebruikt nu ook het echte logo
- `dist` wordt automatisch opnieuw opgebouwd via `npm run build`
