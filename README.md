# Recalled Landing

Minimale Download-Seite für die Recalled App (App Store / Google Play).

## Lokal ansehen

```bash
cd recalled-landing
python3 -m http.server 8080
```

Dann [http://localhost:8080](http://localhost:8080) öffnen.

## App-Links eintragen

In `config.js`:

```js
window.RECALLED_APP = {
  appStoreUrl: "https://apps.apple.com/app/idDEINE_APP_ID",
  playStoreUrl: "https://play.google.com/store/apps/details?id=de.recalled.app",
};
```

Nur die Stores eintragen, die es gibt — leere Felder werden ausgeblendet.

## Auf Render deployen

1. Neues GitHub-Repo erstellen (z. B. `wowarvova/recalled-landing`) und diesen Ordner pushen.
2. Render → **New** → **Blueprint** → Repo verbinden.
3. Oder **New** → **Static Site** → Repo wählen, **Publish directory:** `.`
4. Optional eigene Domain (z. B. `recalled.de` oder `app.recalled.de`) unter **Settings → Custom Domains**.

Kosten: Render **Static Site** ist in der Regel **kostenlos** (Free Tier).

## Partner-Portal

Das Partner-Portal bleibt separat unter `recalled-partner` — Link steht unten auf der Seite.
