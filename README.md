# Confident Minds Foundation &amp; Ontdek Je Brein — websites

Twee statische websites in één repository, klaar voor GitHub Pages:

- **`/confident-minds-foundation/`** — site van de stichting (Confident Minds Foundation).
- **`/ontdek-je-brein/`** — site van het programma Ontdek Je Brein.
- **`/index.html`** — startpagina die naar beide sites verwijst.

De twee sites linken naar elkaar via relatieve paden, dus ze horen in dezelfde repository te blijven.

## Online zetten met GitHub Pages

1. Maak een nieuwe repository aan op GitHub (bv. `ojb-cmf-website`).
2. Push de inhoud van deze map naar de `main`-branch (zie commando's hieronder).
3. Ga in de repository naar **Settings → Pages**.
4. Kies bij *Build and deployment* → *Source*: **Deploy from a branch**, branch **main**, map **/ (root)**. Klik **Save**.
5. Na ~1 minuut is de site live op `https://<gebruikersnaam>.github.io/<repo-naam>/`.

De startpagina verschijnt op de hoofd-URL; de sites staan onder
`/confident-minds-foundation/` en `/ontdek-je-brein/`.

## Lokaal bekijken

Open `index.html` in een browser, of start een lokale server:

```bash
python3 -m http.server 8000
# open daarna http://localhost:8000
```

## Technisch

Pure HTML/CSS, geen build-stap. Het bestand `.nojekyll` zorgt dat GitHub Pages
de bestanden ongewijzigd serveert. Contactformulieren zijn nog placeholders zonder
backend; e-mailadressen moeten nog worden ingevuld.
