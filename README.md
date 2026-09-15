# Fabio è tornato

Sito statico con l'annuncio **"Fabio è tornato. Gioite del ritorno di Fabio."** su sfondo a pioggia
"Matrix": le parole della frase scendono in colonna, a volte nell'ordine giusto, a volte sciolte e slegate.

Il pannello centrale mostra *GIOITE!* e la dicitura generica **Inverno 2027**: nessuna data
precisa, nessun orario.

Online: <https://g95g95.github.io/countdown-biomeccanica/>

## QR code

In basso a destra c'è il QR code del sito (SVG inline, nessuna dipendenza esterna), che punta a
`https://g95g95.github.io/countdown-biomeccanica/`. Le stesse versioni stand-alone, per stampa o
condivisione, sono `qr.svg` e `qr.png`.

Per rigenerarli dopo un cambio di URL:

```bash
pip install segno
python3 -c "import segno; q=segno.make('https://g95g95.github.io/countdown-biomeccanica/', error='m'); \
q.save('qr.svg', scale=10, border=4, dark='#04140a', light='#d9ffe3'); \
q.save('qr.png', scale=12, border=4, dark='#04140a', light='#d9ffe3')"
```

Il QR va tenuto con moduli scuri su fondo chiaro: la versione "verde su nero" è invertita e molti
scanner non la leggono.

## Uso

È un singolo `index.html` senza dipendenze: aprilo nel browser oppure pubblicalo su GitHub Pages.

La dicitura sotto il messaggio è testo statico in `<p id="when">`. Il countdown è fermo sullo
stato finale perché `TARGET` (in `index.html`) è una data passata: per riattivarlo basta metterci
una data futura, in formato ISO con offset del fuso italiano (`+02:00` con ora legale, `+01:00`
con ora solare).
