# Portfolio professionale — Guida per lei (senza scrivere codice)

Questo sito è pensato per essere aggiornato **dal sito web di GitHub**,
senza installare nulla e senza usare comandi. Tre cose si possono
modificare: i testi, le immagini dei lavori, e il CV in PDF.

## Struttura

```
portfolio/
├── index.html      ← la pagina (contiene sia i testi che l'elenco delle opere)
├── images/          ← foto delle opere + foto profilo
└── cv/
    └── cv.pdf       ← il curriculum in PDF
```

## 1. Come modificare i testi (nome, bio, contatti)

1. Vai sulla pagina del repository su github.com.
2. Apri `index.html` e clicca sull'icona a forma di matita ("Edit this file"),
   in alto a destra.
3. Usa **Ctrl+F** (o Cmd+F su Mac) nel browser per trovare velocemente il
   testo da cambiare. Alcuni punti utili da cercare:
   - `Jane Doe` → nome (appare 2 volte: nel menu e nel titolo grande)
   - `Painting & Mixed Media` → la riga sotto il nome
   - `I make paintings and mixed-media work...` → il testo introduttivo
   - `I'm a final-year Fine Art student...` → i due paragrafi della sezione About
   - `[email protected]` → indirizzo email (appare 2 volte, anche nel link)
   - `instagram.com/yourusername` e `linkedin.com/in/yourusername` → i link social
4. Modifica solo il testo tra i simboli `>` e `<` (non toccare i tag HTML
   con le parentesi angolari).
5. In fondo alla pagina, clicca **"Commit changes"** per salvare. Le modifiche
   saranno online dopo circa un minuto.

**Consiglio:** faccia una modifica alla volta e controlli il sito online
prima di continuare, così è facile capire cosa ha cambiato ogni salvataggio.

## 2. Come aggiungere/sostituire un'opera nella galleria

1. Carichi la foto nella cartella `images/` (pulsante "Add file" →
   "Upload files" dentro quella cartella su GitHub).
2. Apra di nuovo `index.html` in modifica.
3. Cerchi `const ARTWORKS = [` verso la fine del file.
4. Copi uno dei blocchi tra `{ }` e lo modifichi:

```js
{
  title: "Titolo dell'opera",
  medium: "Tecnica (es. Oil on canvas)",
  year: "2026",
  image: "images/nome-file.jpg"
}
```

5. Attenzione alla virgola: ogni blocco tranne l'ultimo deve finire con una
   virgola `,` dopo la parentesi graffa `}`.
6. Salvi con "Commit changes".

Se il nome del file scritto in `image:` non corrisponde esattamente al file
caricato (incluse maiuscole/minuscole), al posto della foto apparirà la
scritta "Add image here" con il nome del file mancante — è normale, serve
proprio a farle capire cosa manca.

## 3. Come aggiungere/aggiornare il CV

1. Carichi il PDF nella cartella `cv/`, chiamandolo esattamente `cv.pdf`.
2. Se il nome è diverso, cerchi `cv/cv.pdf` dentro `index.html` (appare 2
   volte) e lo sostituisca con il nome corretto.

## 4. Foto profilo

Stessa logica delle opere: carichi la foto come `images/profile.jpg`
(esattamente questo nome), oppure cerchi `images/profile.jpg` dentro
`index.html` e lo sostituisca con il nome del file che ha caricato.

## Nota sulle immagini

Prima di caricare le foto delle opere, è meglio ridurle di peso così il
sito si carica velocemente. Un sito gratuito e semplicissimo per farlo:
**squoosh.app** — basta trascinare la foto, scaricare il risultato e
caricare quello al posto dell'originale. Circa 1500 pixel sul lato lungo
è più che sufficiente per un portfolio.

## Il sito è già in inglese

Ho scritto tutti i testi della pagina in inglese, così com'era richiesto,
con contenuti d'esempio (nome "Jane Doe", bio generica, ecc.) da sostituire
con le informazioni vere della studentessa seguendo i passaggi sopra.
