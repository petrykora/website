# Astro website template

Kliknij w guzik poniżej, aby zaimportować szalon do *Replit.com*

[![Run on Repl.it](https://replit.com/badge/github/ALOPB-Hack-Club/astro-website-template)](https://replit.com/new/github/ALOPB-Hack-Club/astro-website-template)


## 🚀 Struktura projektu

Szablon składa się z kilku ważnych katalogów, w których umieszczamy pliki.

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Dotatkowo jest kilka katalogów, w których nie umieszczamy kodu.
Są to:
- `.vscode` - pliki pomocnicze programu *Visual Studio Code*
- `node_modules` - pobrane moduły (zależności) projektu
- `dist` - pliki zbudowanej strony, które finalnie umieścimy na serwerze

Astro zwraca uwagę na pliki `.astro` oraz `.md` znajdujące się w katalogu `src/pages/`. Każda strona powinna mieć unikatową nazwę.
Aby zagnieździć (znestować) ścierzkę naszej strony np. `blog/pierwszy-wpis` należy utworzyć katalog. Dodatkowo tworząc plik `index.md` bądź `index.astro` możemy zdefiniować co znajdzie się na samej ścierzce `/blog/`.
```text
pages/
├── index.astro
└── blog/
    ├── index.md          <-- `blog/`    
    └── pierwszy-wpis.md  <-- `blog/pierwszy-wpis/`
```

Wszystkie statyczne zasoby takie jak obrazy czy zdjęcia powinny znaleść się w katalogu `public/`.

## 🧞 Komendy

Możesz wywołać wszystkie komendy w konsoli znajdując się w głównej ścierzce projektu:

| Command                   | Action                                                                   |
| :------------------------ | :----------------------------------------------------------------------- |
| `npm install`             | Instaluje zależności                                                     |
| `npm run dev`             | Włącza lokalny serwer deweloperski `localhost:4321`                      |
| `npm run build`           | Buduje finalną wersję strony do katalogu `./dist/`                       |
| `npm run preview`         | Włącza podgląd finalnej wersji strony (pliki znajdujące się w `./dist/`) |
| `npm run astro ...`       | Wykonuje polecenia frameworka Astro `astro add`, `astro check`           |
| `npm run astro -- --help` | Wyświetla pomoc dotyczącą Astro                                          |

## 👀 Dokumentacja

[Oficjalna dokumntacja Astro ➚](https://docs.astro.build)
