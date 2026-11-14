REPOZYTORIUM DOKUMENTÓW PRAWNYCH LSO

Utwórz osobne PUBLICZNE repozytorium GitHub, np. lsofara-legal.
Skopiuj te dwa pliki do głównego katalogu repozytorium:

  privacy-policy.md
  terms.md

W aplikacji ustaw zmienne serwera:

  LEGAL_CONTENT_REPO=ks0chacki/lsofara-legal
  LEGAL_CONTENT_BRANCH=main

W Vercel: Project → Settings → Environment Variables. Po dodaniu zmiennych
wykonaj jeden redeploy. Na VPS ustaw je w środowisku serwera i zrestartuj
aplikację. Każda odsłona strony sprawdza aktualny plik z GitHuba, więc
późniejsze zmiany są widoczne bez redeployu aplikacji. Zmiana może być
opóźniona o czas propagacji commita po stronie GitHuba (zwykle sekundy).
Gdy GitHub chwilowo nie odpowiada, aplikacja pokaże bezpieczną kopię zapasową.

Pierwszy nagłówek `#` w każdym pliku ustawia tytuł strony. Pozostałe nagłówki
możesz swobodnie zmieniać, dodawać i usuwać w tym repozytorium.

Repozytorium jest publiczne, więc nie dodawaj do niego sekretów ani danych
użytkowników. Jeśli nie ustawisz zmiennych, strona użyje kopii lokalnej.
