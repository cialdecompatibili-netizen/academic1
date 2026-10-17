# academic1

Sito Jekyll (tema Academic Homepage, clone di luost26/academic-homepage) su GitHub Pages: https://cialdecompatibili-netizen.github.io/academic1/

## Cose che funzionano
- Clone in repo propria e Pages attivo con la stessa procedura di arsha1: `gh repo create`, `git clone` del tema, rinomina `origin` in `upstream`, nuovo `origin`, push. In `_config.yml` aggiungere `url` e mettere il nuovo `baseurl` (qui /academic1). Pages si attiva con `gh api -X POST repos/OWNER/NOME/pages --input FILE` dove FILE contiene il JSON della sorgente (main, /).
- Questo tema gira sul build classico di GitHub Pages: il plugin `jekyll-email-protect` del Gemfile non serve al sito (nessun template lo usa).
- Le sottopagine hanno URL senza barra finale (/academic1/blog, /publications, /showcase, /index_layout2): con la barra danno 404.
- In PowerShell usare `\$ProgressPreference='SilentlyContinue'` prima di `Invoke-WebRequest`, altrimenti l'output dei comandi si riempie di righe di avanzamento.
