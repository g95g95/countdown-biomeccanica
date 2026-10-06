# countdown-biomeccanica

Sito statico a file unico (`index.html`, nessuna build). Pubblicato con GitHub Pages dal branch `main`, cartella root.

- Messaggio corrente: "Fabio è tornato. Gioite del ritorno di Fabio." (kicker del pannello, `<title>`, parole della pioggia).
- Nessuna data esposta: sotto il messaggio c'è solo la dicitura generica "Natale 2026", testo statico in `<p id="when">`.
- Data target: costante `TARGET` in `index.html`, ISO con offset esplicito del fuso italiano (CEST `+02:00`, CET `+01:00`). Ora è nel passato, quindi il pannello resta sullo stato finale `GIOITE!`.
- Pioggia Matrix: canvas full-screen; ogni colonna ha 2 gocce a velocità condivisa (mai sovrapposte), ognuna estrae uno "stream" da `makeStream()` (65% frase intera in ordine, 35% 1–3 parole sciolte). `laneW` si misura sulla parola più lunga di `WORDS`.
- Sfondo: `#bg` con `gabibbo.webp` (Gabibbo psichedelico), scurito, in lenta rotazione di tinta (`hue-rotate`) e "respiro"; il canvas della pioggia sfuma verso il trasparente (`destination-out`) per lasciarlo vedere. ~1 stream su 4 è arcobaleno, il resto verde. Bordo del pannello e `GIOITE!` ciclano i colori. Animazioni spente con `prefers-reduced-motion`.
- Pannello countdown: `#panel`, 50vw × 50vh centrato (92vw sotto 760px).
- QR code: `#qr` in basso a destra, SVG inline (nessuna richiesta esterna) verso l'URL Pages; copie stand-alone in `qr.svg` e `qr.png`. Moduli scuri su fondo chiaro, mai invertito.
