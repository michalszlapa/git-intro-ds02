# Zadanie 2: cofanie błędów

1. Dopisz w `notatki.md` bezsensowną linię i **nie** rób commita.
2. Cofnij zmianę: `git restore notatki.md`
3. Teraz dopisz linię, dodaj ją i zrób commit z błędnym komunikatem, np. `"asdf"`.
4. Popraw komunikat ostatniego commita: `git commit --amend -m "Opisowy komunikat"`
5. Sprawdź wynik: `git log --oneline`

**Uwaga:** `--amend` zmienia historię. Rób go tylko na commitach, których nikt jeszcze nie pobrał.
