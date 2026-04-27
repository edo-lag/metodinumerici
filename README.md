# Metodi Numerici per Data Science

Appunti del corso di **Metodi Numerici per Data Science** in formato LaTeX, organizzati come dispensa didattica.

## Contenuto

| File / Cartella | Descrizione |
|---|---|
| `main.tex` | Documento principale (coordina tutti i capitoli) |
| `chapters/chapter01_aritmetica_fp.tex` | Cap. 1 — Aritmetica in virgola mobile, IEEE 754, epsilon di macchina |
| `chapters/chapter02_sistemi_lineari.tex` | Cap. 2 — Sistemi lineari, norme, numero di condizionamento |
| `chapters/chapter03_metodi_diretti.tex` | Cap. 3 — Metodi diretti (eliminazione di Gauss, fattorizzazione LU) |
| `chapters/chapter04_metodi_iterativi.tex` | Cap. 4 — Metodi iterativi (Jacobi, Gauss-Seidel, convergenza) |
| `chapters/chapter05_condizionamento.tex` | Cap. 5 — Condizionamento dei sistemi lineari |
| `images/` | Cartella per le immagini (da aggiungere) |

## Come compilare il PDF

### Opzione 1 — Online con Overleaf (consigliata, nessuna installazione)

1. Vai su [overleaf.com](https://www.overleaf.com) e crea un account gratuito.
2. Clicca **New Project → Upload Project**.
3. Comprimi tutta la cartella del repository in un file `.zip` e caricalo.
4. Clicca **Compile** (▶): il PDF viene generato automaticamente.

### Opzione 2 — Locale con TeX Live (Linux / macOS)

```bash
# Installa TeX Live (se non presente)
sudo apt install texlive-full   # Debian/Ubuntu
# oppure
brew install --cask mactex      # macOS

# Compila (esegui due volte per indice e riferimenti incrociati)
pdflatex main.tex
pdflatex main.tex
```

### Opzione 3 — Locale con MiKTeX (Windows)

1. Installa [MiKTeX](https://miktex.org/download).
2. Apri `main.tex` con TeXworks (incluso in MiKTeX).
3. Seleziona **pdfLaTeX** e premi il tasto di compilazione.

## Struttura sorgente LaTeX

```
metodinumerici/
├── main.tex               ← documento principale
├── chapters/
│   ├── chapter01_aritmetica_fp.tex
│   ├── chapter02_sistemi_lineari.tex
│   ├── chapter03_metodi_diretti.tex
│   ├── chapter04_metodi_iterativi.tex
│   └── chapter05_condizionamento.tex
├── images/                ← immagini (PNG, PDF, EPS)
└── README.md
```

## Argomenti trattati

- **Aritmetica in virgola mobile**: standard IEEE 754, numeri di macchina, troncamento e arrotondamento, epsilon di macchina, algoritmo di Horner, propagazione degli errori.
- **Sistemi lineari**: rappresentazione matriciale, spazi vettoriali, norme vettoriali e matriciali, numero di condizionamento.
- **Metodi diretti**: sistemi triangolari, fattorizzazione LU, eliminazione di Gauss, pivoting.
- **Metodi iterativi**: splitting della matrice, Jacobi, Gauss-Seidel, criteri di convergenza, dominanza diagonale.
- **Condizionamento**: perturbazione dei dati, errore relativo, backward/forward error.
