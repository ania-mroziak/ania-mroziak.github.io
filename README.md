# Portfolio Ani Mroziak (repozytorium prywatne)

Strona-portfolio Social Media Managerki: realizacje dla Uzdrovisco, Pantalones, marek beauty i modowych, Rozwojowej Mamy, archiwum Mentos i Chupa Chups oraz zespół agentów AI.

> 🔒 Repozytorium musi zostać **prywatne**.

## Jak obejrzeć
Otwórz `index.html` w przeglądarce (dwuklik po pobraniu repozytorium). Strona działa bez internetu, poza linkami do Instagrama.

## Co jest gdzie
| Folder | Zawartość |
|---|---|
| `index.html` | cała strona: tekst, układ, style i skrypty |
| `media/` | kadry i filmy z dźwiękiem (rolki, pętle, okładki) |
| `img/` | zrzuty feedu i dodatkowe kadry |
| `logos/` | oryginalne logotypy marek |
| `fonts/` | font Beaulieu |
| `video/` | film Doctor Brew |

## Zasady treści
- Wszystkie liczby to publiczne dane z Instagrama, oznaczone jako wyniki organiczne. Pupa Milano bez liczb.
- Komentarze obserwatorek bez nazw kont; bez komentarzy Ani i zespołów marek.

## Bezpieczeństwo
- Hook `pre-commit` (gitleaks i własne wzorce) blokuje commit z kluczem lub tokenem. Włączenie: `git config core.hooksPath .githooks`.
- Workflow „Kontrola” skanuje całą historię gitleaksem przy każdej wysyłce i co poniedziałek oraz sprawdza konfigurację Renovate.
- Renovate aktualizuje przypięte akcje GitHuba. Szczegóły: [SECURITY.md](SECURITY.md).
