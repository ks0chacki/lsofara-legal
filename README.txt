REPOZYTORIUM DOKUMENTÓW PRAWNYCH LSO

Utwórz osobne PUBLICZNE repozytorium GitHub, np. lsofara-legal.
Skopiuj te dwa pliki do głównego katalogu repozytorium:

  privacy-policy.md
  terms.md

W aplikacji ustaw zmienne serwera:

  LEGAL_CONTENT_REPO=NAZWA_UZYTKOWNIKA/lsofara-legal
  LEGAL_CONTENT_BRANCH=main

W Vercel: Project → Settings → Environment Variables. Po dodaniu zmiennych
wykonaj jeden redeploy. Na VPS ustaw je w środowisku serwera i zrestartuj
aplikację. Późniejsze edycje plików w GitHubie pojawią się po wygaśnięciu
pięciominutowej pamięci podręcznej; nie wymagają redeployu aplikacji.

Repozytorium jest publiczne, więc nie dodawaj do niego sekretów ani danych
użytkowników. Jeśli nie ustawisz zmiennych, strona użyje kopii lokalnej.
