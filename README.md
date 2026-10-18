# Postavljanje (bez Apps Scripta)

## 1. Drive mape
Galerija, Video i PDF moraju biti dijeljene kao **Svi s poveznicom → Preglednik**.
Podmape su tabovi na stranici. Sve što ubaciš vidi se **odmah** nakon osvježavanja stranice.

## 2. Google API ključ (5 min, besplatno)
1. console.cloud.google.com → novi projekt "koncept-zdravlje".
2. **APIs & Services → Library → Google Drive API → Enable**.
3. **APIs & Services → Credentials → Create credentials → API key**.
4. Klikni na ključ → **Restrict key**:
   - Application restrictions: **Websites**, dodaj `https://sbatinac.github.io/*` (Rebrandly samo preusmjerava, njega ne treba dodavati).
   - API restrictions: **Restrict key → Google Drive API**.
5. Kopiraj ključ u `index.html` → `const DRIVE_KEY = '...'`.

Ključ je vidljiv u kodu, ali je zaključan na tvoju stranicu i samo na čitanje javnih Drive datoteka. To je standardna praksa.

## 3. Kontakt forma (FormSubmit)
1. Nakon objave pošalji jedan probni upit s forme.
2. FormSubmit šalje mail za aktivaciju na kristina505@gmail.com → klikni **Activate**.
3. Od tada svi upiti stižu na taj mail.
4. (Opcionalno) U aktivacijskom mailu dobiješ tajni kod. Upiši ga umjesto emaila u `FORM_EMAIL` da adresa ne bude vidljiva u kodu.

## 4. GitHub Pages
1. Repo `koncept-zdravlje` → upload `index.html` (+ `banner.jpg`).
2. Settings → Pages → Branch: `main` / root → Save.
3. Stranica: `https://sbatinac.github.io/koncept-zdravlje/`

## 5. Rebrandly
Novi link → Destination: `https://sbatinac.github.io/koncept-zdravlje/` → odaberi svoj branded slug.
