# Fanaberie Kulinarne Piotra Senatora

## O projekcie

Witaj w "Fanaberiach Kulinarnych" – mojej osobistej kolekcji domowych przepisów, sezonowych smaków i czasem nieco szalonych kulinarnych eksperymentów. Ta strona to przestrzeń, gdzie dzielę się tym, co wychodzi z piekarnika i z patelni, a także luźnymi notatkami z kuchni, które zbieram od lat.

Gotowanie dla bliskich to dla mnie przyjemność, a nie obowiązek. Znajdziesz tu klasyczne dania, pomysły na wykorzystanie sezonowych składników i kilka nietypowych zachcianek. Nie ma ambicji na mistrzostwa, jest za to miejsce na improwizację, wspomnienia i kaprys.

Strona została zbudowana przy użyciu **Jekylla** i jest hostowana na **GitHub Pages**, co zapewnia szybkość, prostotę i łatwość zarządzania.

## Zobacz stronę na żywo

Odwiedź "Fanaberie Kulinarne" pod adresem:
[https://kuchnia.senator.lu](https://kuchnia.senator.lu)

## Struktura projektu

Projekt jest zorganizowany w oparciu o kolekcje Jekylla, co ułatwia dodawanie nowych treści:

* `_config.yml`: Główny plik konfiguracyjny Jekylla.
* `_layouts/`: Szablony HTML definiujące układ strony (np. `default.html`, `recipe.html`, `note.html`).
* `_includes/`: Mniejsze, wielokrotnie używane fragmenty kodu HTML (np. `header.html`, `footer.html`, `recipe_card.html`).
* `assets/`: Zawiera pliki CSS (`assets/css/style.css`), JavaScript (`assets/js/main.js`) oraz niestandardowe fonty (`assets/fonts/`).
* `_data/categories.yml`: Plik danych definiujący wszystkie kategorie przepisów.
* `_recipes/`: Kolekcja zawierająca wszystkie przepisy w formacie Markdown (`.md`).
* `_notes/`: Kolekcja zawierająca wszystkie notatki z kuchni w formacie Markdown (`.md`).
* `images/`: Folder na wszystkie grafiki, podzielony na:
    * `images/recipes/`: Główne zdjęcia przepisów (proporcje 4:3).
    * `images/notes/`: Zdjęcia do notatek (proporcje 4:3).
    * `images/general/`: Ogólne grafiki, takie jak placeholder czy obrazki do strony 404.
* `categories/`: Statyczne strony dla każdej z kategorii, które dynamicznie listują przepisy.
* `index.html` (lub `index.md`): Strona główna.
* `404.html`: Strona błędu "nie znaleziono".

## Jak uruchomić lokalnie?

Aby uruchomić projekt na swoim komputerze:

1.  **Wymagania:** Upewnij się, że masz zainstalowane Ruby, Bundler i Jekyll. Jeśli nie, postępuj zgodnie z instrukcjami na [oficjalnej stronie Jekylla](https://jekyllrb.com/docs/installation/).
2.  **Klonowanie repozytorium:**
    ```bash
    git clone [https://github.com/TwojaNazwaUzytkownika/kuchnia.senator.lu.git](https://github.com/TwojaNazwaUzytkownika/kuchnia.senator.lu.git)
    cd kuchnia.senator.lu
    ```
    (Zastąp `TwojaNazwaUzytkownika` swoją rzeczywistą nazwą użytkownika GitHub.)
3.  **Instalacja zależności:**
    ```bash
    bundle install
    ```
4.  **Uruchomienie serwera Jekylla:**
    ```bash
    bundle exec jekyll serve
    ```
    Strona będzie dostępna pod adresem `http://localhost:4000` (lub innym wskazanym w konsoli).

## Jak dodawać nowe treści?

* **Przepisy:** Utwórz nowy plik Markdown (`.md`) w folderze `_recipes/`. Użyj formatu `nazwa-przepisu.md` i pamiętaj o dodaniu odpowiedniego **front matter** (np. `title`, `category`, `time`, `portions`, `difficulty`, `image_main`, `description`). Treść przepisu (składniki, przygotowanie) pisz bezpośrednio w Markdownie.
* **Notatki:** Utwórz nowy plik Markdown (`.md`) w folderze `_notes/`. Nazwij go w formacie `YYYY-MM-DD-nazwa-notatki.md` i dodaj **front matter** (np. `title`, `date`, `image_main`). Treść notatki pisz w Markdownie.
* **Zdjęcia:** Umieszczaj zdjęcia przepisów w `images/recipes/` i zdjęcia notatek w `images/notes/`. Pamiętaj, że wszystkie zdjęcia są w proporcjach **4:3**.

## Licencja

Ten projekt jest udostępniony na licencji [MIT](https://opensource.org/licenses/MIT).
