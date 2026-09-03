# Countdown visita biomeccanica — piano

Obiettivo: sito statico con countdown a **venerdì 4 settembre 2026, ore 9:30 (Europe/Rome)**,
pannello centrale che occupa metà schermo, sfondo a pioggia "Matrix" di parole tratte dalla frase
"Ore 9:30 visita biomeccanica Brian's il grande ciclismo" (a volte in ordine, a volte staccate).
Pubblicazione su repo GitHub dedicato + GitHub Pages.

## Task
- [ ] 1. `index.html` unico (HTML + CSS + JS inline, nessuna dipendenza esterna)
  - [ ] countdown (giorni se >0, ore, minuti, secondi) con target in fuso italiano fisso
  - [ ] pannello 50vw × 50vh centrato, responsive su mobile
  - [ ] canvas full-screen con pioggia di parole: ~65% frase intera in ordine, ~35% 1–3 parole sciolte
  - [ ] stato "È ORA!" al raggiungimento
- [ ] 2. Verifica locale (screenshot headless con Edge)
- [ ] 3. `README.md` + `CLAUDE.md` minimale
- [ ] 4. `git init` → repo GitHub pubblico `countdown-biomeccanica` → push
- [ ] 5. Abilita GitHub Pages (branch main, root) e verifica URL raggiungibile

## Note
- Target hard-coded come `2026-09-04T09:30:00+02:00` (CEST): corretto per settembre, indipendente dal fuso del visitatore.
- Repo pubblico: necessario per GitHub Pages su account free.
