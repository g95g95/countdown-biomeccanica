# countdown-biomeccanica

Sito statico a file unico (`index.html`, nessuna build). Pubblicato con GitHub Pages dal branch `main`, cartella root.

- Messaggio corrente: "Fabio è tornato. Gioite del ritorno di Fabio." (kicker del pannello, `<title>`, parole della pioggia).
- Data target: costante `TARGET` in `index.html`, ISO con offset esplicito del fuso italiano (CEST `+02:00`, CET `+01:00`).
- Pioggia Matrix: canvas full-screen; ogni colonna ha 2 gocce a velocità condivisa (mai sovrapposte), ognuna estrae uno "stream" da `makeStream()` (65% frase intera in ordine, 35% 1–3 parole sciolte). `laneW` si misura sulla parola più lunga di `WORDS`.
- Pannello countdown: `#panel`, 50vw × 50vh centrato (92vw sotto 760px).
- QR code: `#qr` in basso a destra, SVG inline (nessuna richiesta esterna) verso l'URL Pages; copie stand-alone in `qr.svg` e `qr.png`. Moduli scuri su fondo chiaro, mai invertito.
