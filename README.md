# Sveska

Statički sajt (GitHub Pages) za objavljivanje zadataka sa slikama. Zadaci se čuvaju u `entries.json`, a slike u folderu `images/`.

Sajt: https://eskicmateja.github.io/sveska/

## Stranice

- `index.html` – početna strana
- `zadaci.html` – lista svih zadataka
- `upload.html` – dodavanje i brisanje zadataka

## Dodavanje zadataka

Zadaci se dodaju preko `upload.html`. Stranica piše direktno u ovaj repo preko GitHub API-ja (grana `main`), pa joj treba GitHub **fine-grained personal access token**:

1. GitHub → Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token.
2. Repository access: *Only select repositories* → `EskicMateja/sveska`.
3. Permissions → Repository permissions → **Contents: Read and write**.
4. Token nalepi u `upload.html`. Čuva se samo u tom browseru (localStorage).

## Uključivanje GitHub Pages

Settings → Pages → Build and deployment → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)` → Save.

## Podešavanje

Vlasnik i ime repoa su na jednom mestu, u `config.js`.
