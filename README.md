# Pucek Reps — GitHub + Pages CMS + Netlify

Ta paczka jest gotowa do wrzucenia do repozytorium GitHub. Netlify nadal jest hostingiem strony. Pages CMS służy tylko jako prosty panel do dodawania produktów.

## 1. Wrzucenie na GitHub

W repozytorium GitHub wybierz **uploading an existing file** i przeciągnij **wszystkie pliki i foldery z tej paczki**. Ważne, żeby `.pages.yml` był w głównym katalogu repozytorium obok `index.html`.

## 2. Pages CMS

1. Wejdź na `https://app.pagescms.org/`.
2. Zaloguj się przez GitHub.
3. Zezwól Pages CMS na dostęp do repozytorium Pucek Reps.
4. Otwórz repozytorium.
5. Powinna pojawić się sekcja **Produkty Pucek Reps**.

W formularzu możesz podać nazwę, zdjęcie, cenę, walutę, jedną lub kilka kategorii, USFans, Weidian oraz włączyć Best Finds i wpisać numer.

## 3. Netlify

W istniejącym projekcie Netlify podepnij repozytorium GitHub jako źródło wdrożeń. Nie twórz nowego projektu, jeśli chcesz zachować obecny adres i ustawienia.

Ustawienia dla tej paczki:
- Build command: zostaw puste
- Publish directory: `.`
- Branch: `main`

Po zapisaniu produktu w Pages CMS zmiana trafia do GitHuba, a Netlify publikuje nową wersję strony.

## Jak działa dodawanie produktu

Pages CMS zapisuje produkty do `data/cms-products.json`, a `index.html` automatycznie wczytuje ten plik. Nie trzeba ręcznie edytować kodu strony.
