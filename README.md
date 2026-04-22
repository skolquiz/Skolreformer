# Skolreformer · Grundskola, förskola & fritidshem

Interaktiv tidsordnad översikt av de största skolreformerna i Sverige, med fokus på grundskola, förskola och fritidshem. Varje reform har utfällbara ansvarspunkter för **skolchef/huvudman** och **rektor**, med paragrafhänvisningar och direktlänkar till propositioner på riksdagen.se.

---

## Snabbstart: deploya till GitHub Pages

### Om du inte har ett repo ännu

```bash
# 1. Skapa ett nytt repo på github.com först (t.ex. "skolreformer-moa")
# 2. I terminalen, i mappen där index.html och README.md ligger:

git init
git add index.html README.md
git commit -m "Initial version: skolreformer-översikt"
git branch -M main
git remote add origin https://github.com/<ditt-användarnamn>/<repo-namn>.git
git push -u origin main
```

### Om du redan har ett repo

```bash
# Kopiera in index.html och README.md i din lokala repo-mapp, sedan:

git add index.html README.md
git commit -m "Uppdatera skolreformer-översikt"
git push
```

### Aktivera GitHub Pages

1. Gå till repot på github.com.
2. **Settings → Pages**.
3. Under *Source*: välj **Deploy from a branch**.
4. Välj branch `main` och folder `/ (root)`. Tryck *Save*.
5. Efter 1–2 minuter publiceras sidan på `https://<ditt-användarnamn>.github.io/<repo-namn>/`.

---

## Stack

- Ren HTML + CSS + vanilla JS — inget bygge, inga beroenden
- Fonter: Fraunces (display) + IBM Plex Sans (body) + IBM Plex Mono (teknisk) via Google Fonts CDN
- Allt ligger inline i `index.html` (~95 kB)

## Struktur

- **Hero** — intro
- **Sticky år-nav** — 2026 · 2027 · 2028 · Pågående
- **Tidslinje** — reformkort i kronologisk ordning per år, med utfällbara accordion-punkter och källhänvisningar till konkreta paragrafer
- **Pågående utredningar** — SOU:er som ännu inte blivit propositioner
- **Källhub** — centrala sidor att bevaka

## Underhåll

När en ny proposition eller SOU tillkommer, lägg till ett nytt `<article class="reform">` under rätt år. Följ mönstret som redan finns — inklusive accordion-strukturen (`role-item` → `role-item-toggle` → `role-item-body`) med paragrafreferens i `role-item-source`.

---

Senast uppdaterad: april 2026
