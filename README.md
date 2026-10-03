# PARKET MONT ILIĆ - sajt

## Struktura
- `index.html` - sajt
- `support.js` - runtime (obavezan, ne brisati)
- `image-slot.js` - prikaz fotografija
- `assets/logo-mark.png` - logo
- `assets/images/` - fotografije (spisak imena u assets/images/README.md)
- `.nojekyll` - isključuje Jekyll obradu na GitHub Pages

## Objava na GitHub Pages
1. Napravite novi repozitorijum na GitHub-u.
2. Prebacite SADRŽAJ ovog foldera u koren repozitorijuma (Add file → Upload files, ili git push).
3. Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save.
4. Sajt je za minut-dva na `https://<korisnik>.github.io/<repo>/`.

Lokalno testiranje: sajt mora da se otvori preko servera (ne dvoklikom), npr. `npx serve .` ili `python -m http.server`.

## Pre objave
- Ubacite fotografije u `assets/images/`.
- Kontakt forma ne šalje e-mail; povežite je sa servisom (npr. Formspree: dodajte action="https://formspree.io/f/XXXX" i method="POST" na <form>).
- Oznake "klijent treba da dostavi/potvrdi" se gase u index.html: u data-props JSON promenite "showNotes" default na false, ili uklonite te elemente.
