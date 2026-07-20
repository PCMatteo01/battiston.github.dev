# Portfolio — starter scaffold

## Struttura (multipagina)
```
index.html            → Home
about.html             → About
portfolio.html          → Portfolio con filtri (PC / VR / 3D Model)
offtopic.html           → Offtopic
project-example.html  → Template pagina di dettaglio progetto (duplicala per ogni progetto)
css/style.css         → Tutto lo stile (design system "blueprint"), condiviso da tutte le pagine
js/main.js            → Logica del filtro portfolio (usata solo in portfolio.html)
assets/               → Metti qui le tue immagini/video
```

⚠️ La sidebar (nome, contatti, menu) è duplicata identica in ogni pagina HTML.
Se cambi nome, email o link, aggiornali in **tutti** i file (index, about, portfolio, offtopic, project-example e ogni pagina progetto che crei).

## Come pubblicarlo su GitHub Pages

1. Crea un repository chiamato **esattamente** `tuousername.github.io`
2. Carica dentro tutti i file di questa cartella (mantenendo le sottocartelle css/ e js/)
3. Vai su Settings → Pages e verifica che il branch `main` sia selezionato come source
4. Dopo qualche minuto il sito sarà live su `https://tuousername.github.io`

## Cosa personalizzare

- **Nome e contatti**: sidebar in `index.html` e `project-example.html` (sono duplicati, tienili sincronizzati)
- **Testo Home/About**: sezioni `#home` e `#about` in `index.html`
- **Progetti**: duplica il blocco `<article class="project-card">` per ogni progetto, aggiorna `data-tags` (usa `pc`, `vr`, `3d` — puoi combinarli tipo `data-tags="pc vr"`), immagine, titolo, descrizione, link
- **Immagini/video**: metti i file in `assets/`, poi nel posto dove vedi `IMAGE / VIDEO PLACEHOLDER` sostituisci con:
  ```html
  <img src="assets/nome-immagine.jpg" alt="Descrizione">
  ```
  o per un video:
  ```html
  <video src="assets/nome-video.mp4" controls></video>
  ```
- **Pagina progetto**: duplica `project-example.html` per ogni progetto (es. `project-nomegioco.html`) e aggiorna i link nelle card di `index.html`

## Note
- Nessuna build scaricabile o WebGL giocabile: solo immagini/video + testo, come richiesto.
- Font caricati da Google Fonts (Space Grotesk, IBM Plex Sans, IBM Plex Mono) — nessuna installazione necessaria.
- Il sito è responsive e rispetta `prefers-reduced-motion`.
