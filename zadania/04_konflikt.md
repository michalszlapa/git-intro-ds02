# Zadanie 4: konflikt

Plik `konflikt/przepis.md` jest w `main`. Zrobisz konflikt celowo, żeby go rozwiązać.

1. Utwórz gałąź `wersja-a`: `git switch -c wersja-a`
2. W `konflikt/przepis.md` zmień **pierwszą** linię na coś innego, zrób commit.
3. Wróć na `main`: `git switch main`
4. Utwórz gałąź `wersja-b`: `git switch -c wersja-b`
5. W tej samej linii wpisz **inną** zmianę, zrób commit.
6. Wróć na `main` i scal `wersja-a`: `git merge wersja-a`
7. Scal `wersja-b`: `git merge wersja-b`. Git zgłosi konflikt.
8. Otwórz plik. Zobaczysz znaczniki `<<<<<<<`, `=======`, `>>>>>>>`.
9. Usuń znaczniki, zostaw wersję, którą uważasz za właściwą (albo połącz obie).
10. `git add konflikt/przepis.md` i `git commit`

**Pytanie:** co się stanie, gdy zmienisz różne linie w obu gałęziach?
