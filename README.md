# drcommodo.it

Sito del Dr. Mario Commodo, Cardiochirurgo e Cardiologo – Novara.
Sito statico in un solo file (`index.html`), senza CMS e senza dipendenze.

## Struttura

- `index.html` – tutto il sito (HTML, CSS e JS)
- `img/` – foto del medico e dello studio (da aggiungere)
- `vercel.json` – impostazioni Vercel (URL puliti, intestazioni di sicurezza, cache immagini)
- `robots.txt`, `sitemap.xml` – per Google

## Pubblicazione su Vercel

1. Carica questa cartella in un repository GitHub (es. `drcommodo`).
2. Su vercel.com: **Add New → Project → Import** il repository. Framework: **Other**. Nessun comando di build. Deploy.
3. Il sito è subito online su un indirizzo `*.vercel.app`.
4. Per il dominio: **Project → Settings → Domains → Add** `drcommodo.it` e `www.drcommodo.it`. Vercel mostra i record DNS da inserire presso il registrar del dominio (di solito un record A `76.76.21.21` per il dominio principale e un CNAME `cname.vercel-dns.com` per `www`). SSL è automatico.
5. Ogni volta che si fa un commit su GitHub, Vercel ripubblica il sito da solo.

## Aggiornare le foto

Mettere i file in `img/` e sostituire i tre blocchi segnaposto in `index.html` (cercare il commento `FOTO REALE`):

- `img/ritratto.jpg` – 800×1000 px
- `img/dottore-2.jpg` – 800×1000 px
- `img/studio.jpg` – 1200×675 px

L'immagine di repertorio nella sezione Prestazioni si elimina cancellando il blocco `<figure class="stock" data-removibile="true">`.

## Da completare prima di andare online

Cercare `[DA CONFERMARE]` in `index.html`: numero Ordine dei Medici, P.IVA, codice fiscale, sede e anno delle specializzazioni, link alla scheda Google Business Profile, link WEBPERVOI, data della privacy policy.
