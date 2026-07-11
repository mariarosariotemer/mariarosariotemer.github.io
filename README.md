# Portfolio professionale — Guida per lei (senza scrivere codice)

Questo sito è pensato per essere aggiornato **dal sito web di GitHub**,
senza installare nulla e senza usare comandi. Il sito mostra le sue
ricerche e analisi come **PDF** (non foto di opere), pensato per una
studentessa di Art Market / Art Business.

## Struttura

```
portfolio/
├── index.html      ← la pagina (testi + elenco delle ricerche)
├── images/
│   └── profile.jpg  ← foto profilo (sezione About)
├── papers/          ← qui vanno i PDF di ricerche, analisi, case study
└── cv/
    └── cv.pdf       ← il curriculum in PDF
```

## 1. Come modificare i testi (nome, bio, contatti)

1. Vai sulla pagina del repository su github.com.
2. Apri `index.html` e clicca sull'icona a forma di matita ("Edit this file").
3. Usa **Ctrl+F** (o Cmd+F su Mac) per trovare velocemente il testo da
   cambiare. Punti utili da cercare:
   - `Jane Doe` → nome (appare 2 volte)
   - `Art Market Analysis` → riga sotto il nome
   - `I research and write about...` → testo introduttivo
   - `I'm a final-year student...` → i due paragrafi della sezione About
   - `[email protected]` → email (appare 2 volte)
   - `instagram.com/yourusername`, `linkedin.com/in/yourusername` → link social
4. Modifichi solo il testo tra `>` e `<` (non tocchi i tag HTML con le
   parentesi angolari).
5. In fondo alla pagina, clicchi **"Commit changes"** per salvare.

**Consiglio:** una modifica alla volta, controllando il sito online dopo
ogni salvataggio.

## 2. Come aggiungere una nuova ricerca/analisi (PDF)

1. Carichi il PDF nella cartella `papers/` ("Add file" → "Upload files").
2. Apra `index.html` in modifica.
3. Cerchi `const PAPERS = [` verso la fine del file.
4. Copi uno dei blocchi tra `{ }` e lo modifichi:

```js
{
  title: "Titolo della ricerca",
  category: "Market Analysis",   // es: Case Study, Market Research, Data Analysis
  date: "2026-07",                // anno-mese, es: 2026-07
  description: "Una o due frasi che spiegano di cosa parla il documento.",
  file: "papers/nome-del-file.pdf"
}
```

5. Attenzione alla virgola: ogni blocco tranne l'ultimo deve finire con
   una virgola `,` dopo la parentesi graffa `}`.
6. Salvi con "Commit changes".

Le ricerche vengono mostrate nell'ordine in cui compaiono nella lista
`PAPERS` — se vuole un ordine diverso, sposti i blocchi.

## 3. Come aggiornare il CV

Carichi il PDF nella cartella `cv/` chiamandolo esattamente `cv.pdf`.
Se usa un nome diverso, cerchi `cv/cv.pdf` dentro `index.html` (appare
2 volte) e lo sostituisca.

## 4. Foto profilo

Carichi la foto come `images/profile.jpg` (esattamente questo nome),
oppure cerchi `images/profile.jpg` dentro `index.html` e lo sostituisca
con il nome del file caricato.

## Nota sui PDF

Non c'è un limite stretto, ma per un caricamento veloce del sito è meglio
evitare PDF enormi con tante immagini ad altissima risoluzione — se un
documento pesa più di qualche decina di MB, conviene comprimerlo prima
di caricarlo (esistono strumenti online gratuiti come Smallpdf o iLovePDF
per comprimere i PDF).

## Il sito è già in inglese

Ho scritto tutti i testi in inglese come richiesto, con contenuti
d'esempio (nome "Jane Doe", bio generica, quattro ricerche di esempio a
tema mercato dell'arte) da sostituire con le informazioni vere della
studentessa seguendo i passaggi sopra.
