# Model Sticlă

Calculator simplu pentru pozițiile dungilor de pe un geam. Merge pe orice telefon, din browser, și poate fi pus pe ecranul principal ca aplicație (funcționează și fără internet).

## Cum se calculează

Spațiile sunt egale sus, jos și între dungi:

```
spațiu = (înălțime − număr_dungi × grosime) / (număr_dungi + 1)
```

Toate cotele din tabel se măsoară de la **marginea de sus** a geamului (de unde începe și unde se termină fiecare dungă).

Modele:
1. **Alternant** – dungi scurte, pe rând din dreapta și din stânga.
2. **Aliniat** – dungi scurte, toate din aceeași parte.
3. **Lățime totală** – dungi pe toată lățimea geamului.

## Publicare (GitHub Pages)

1. Urcă repo-ul pe GitHub.
2. Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. După ~1 minut aplicația e la `https://<utilizator>.github.io/ModelSticla/`.
4. Pe telefon: deschide linkul → meniul browserului → „Adaugă pe ecranul de pornire”.

La fiecare modificare a fișierelor, crește versiunea `CACHE` din `sw.js`.

## Rulare locală

```
python -m http.server 8765
```
