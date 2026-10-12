# Ściągawka: git

## Podstawy
| Komenda | Co robi |
|---|---|
| `git status` | pokazuje stan plików |
| `git diff` | zmiany niezapisane w poczekalni |
| `git diff --staged` | zmiany w poczekalni (gotowe do commita) |
| `git add <plik>` | dodaje plik do poczekalni |
| `git commit -m "opis"` | zapisuje commit |
| `git log --oneline` | historia commitów |

## Cofanie
| Komenda | Co robi |
|---|---|
| `git restore <plik>` | odrzuca niezapisane zmiany w pliku |
| `git restore --staged <plik>` | wyjmuje plik z poczekalni |
| `git commit --amend` | poprawia ostatni commit (tylko lokalny!) |

## Gałęzie
| Komenda | Co robi |
|---|---|
| `git switch -c <nazwa>` | tworzy i przełącza gałąź |
| `git switch main` | wraca na main |
| `git merge <gałąź>` | scala gałąź do bieżącej |
| `git branch -d <gałąź>` | usuwa scaloną gałąź |

## Zdalne
| Komenda | Co robi |
|---|---|
| `git push` | wysyła commity na GitHuba |
| `git push -u origin <gałąź>` | wysyła nową gałąź i ustawia śledzenie |
| `git pull` | pobiera i scala zmiany z GitHuba |
| `git fetch` | pobiera zmiany, ale nic nie scala |

## Gdy coś poszło nie tak
- **Konflikt przy merge:** `git merge --abort` wraca do stanu sprzed merge.
- **Pomyliłem gałąź:** `git log --oneline --all` pokaże, gdzie są commity.
- **Chcę zobaczyć, co się dzieje:** `git status` zawsze jest bezpieczne.
- **Zgubiłem commit:** `git reflog` pokazuje wszystkie wcześniejsze pozycje HEAD.
