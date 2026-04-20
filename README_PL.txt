OVERBOT MOBILE APK — instrukcja

Co to jest:
To pełny projekt Android Studio dla aplikacji APK. Appka otwiera lokalny panel OverBot i pozwala skanować mecze po wklejeniu klucza API-Football.

WAŻNE:
W tym środowisku nie dało się uczciwie zbudować gotowego APK, bo brakuje Android SDK i build tools.
Dlatego dostajesz gotowy projekt APK + workflow GitHub Actions, który sam zbuduje APK w chmurze.

OPCJA 1 — Android Studio:
1. Rozpakuj ZIP.
2. Otwórz folder projektu w Android Studio.
3. Poczekaj aż Gradle dociągnie zależności.
4. Kliknij Build > Build APK(s).
5. Gotowy plik znajdziesz w:
   app/build/outputs/apk/debug/

OPCJA 2 — GitHub bez instalowania Android Studio:
1. Załóż nowe prywatne repo na GitHub.
2. Wrzuć tam cały rozpakowany projekt.
3. Wejdź w zakładkę Actions.
4. Uruchom workflow "Build APK".
5. Po zakończeniu pobierz artifact: overbot-debug-apk.
6. W środku będzie plik APK do instalacji na Androidzie.

CO ROBI APPKA:
- zapisuje klucz API lokalnie w telefonie,
- pozwala ustawić datę i próg score,
- ma tryb demo,
- skanuje ligi wpisane w JSON,
- liczy prosty score pod over 4.5 / 5.5 / 6.5.

UWAGA:
- klucz API jest używany bezpośrednio w appce, więc traktuj ją jako prywatną wersję dla siebie,
- jeśli chcesz, mogę później zrobić wersję z Telegram alertami i backendem, wtedy będzie solidniejsza.
