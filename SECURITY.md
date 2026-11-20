# Bezpieczeństwo

## Zasady
- Repozytorium jest **publiczne** (decyzja Ani z 20.11.2026), bo z niego działa strona GitHub Pages. Nie trafiają tu materiały objęte NDA ani dane, których nie ma w publicznych postach.
- **Do repo nigdy nie trafiają** klucze, tokeny, hasła ani pliki `credentials.json` / `token*.json`. Pilnują tego `.gitignore`, hook `pre-commit` (gitleaks i własne wzorce) oraz skan gitleaks w GitHub Actions przy każdej wysyłce i co tydzień.
- GitHub Actions działają z minimalnymi uprawnieniami (`contents: read`), a akcje są przypięte do konkretnych commitów (SHA). Ich aktualizacje przychodzą od Renovate.
- Historii nie przepisujemy: żadnego `git push --force`.

## Co zrobić, jeśli klucz trafił do repo
Samo usunięcie pliku nie wystarczy, bo klucz zostaje w historii. Najpierw trzeba go **unieważnić** u dostawcy (procedury: `claude-ania-baza/SECURITY.md`), potem usunąć z pliku. Czyszczenie historii tylko po decyzji Ani.
