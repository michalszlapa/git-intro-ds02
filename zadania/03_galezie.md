# Zadanie 3: gałęzie

1. Utwórz i przełącz się na nową gałąź: `git switch -c dodaj-sekcje`
2. Dopisz w `notatki.md` nową sekcję `## Gałęzie` z jednym zdaniem.
3. Zrób commit na tej gałęzi.
4. Wróć na `main`: `git switch main`
5. Zobacz, że sekcji tam nie ma.
6. Scal gałąź: `git merge dodaj-sekcje`
7. Usuń gałąź: `git branch -d dodaj-sekcje`

**Pytanie:** dlaczego po powrocie na `main` sekcja zniknęła z pliku?
