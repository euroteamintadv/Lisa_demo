# Lisa — Landing Page

**Assistente digitale per anziani** — your friendly AI companion  
Landing page one-pager con scroll-snap

## 🔗 Links

- **Live**: https://mylisa.net
- **Repo**: https://github.com/euroteamintadv/Lisa_demo
- **Actions**: https://github.com/euroteamintadv/Lisa_demo/actions
- **Preview (branch)**: `https://htmlpreview.github.io/?https://github.com/euroteamintadv/Lisa_demo/blob/PREVIEW_BRANCH/index.html`

## 🛠 Stack

- **HTML + CSS puro** — single file, zero dipendenze
- **GitHub Pages** — hosting + HTTPS automatico
- **GitHub Actions** — deploy su push (`pages build and deployment`)

## 🎨 Design System

| Token | Valore | Uso |
|---|---|---|
| `--rosa` | `#D4849A` | Accenti, icone, badge |
| `--rosa-chiaro` | `#F7EAED` | Sfondi alternati |
| `--azzurro` | `#E3EEF2` | Sfondi alternati |
| `--grigio-caldo` | `#4A4440` | Titoli (contrasto 4.5:1+) |
| `--grigio-medio` | `#7A7270` | Testi secondari |
| `--bianco` | `#FFFFFF` | Sfondo principale |
| `--nero-testo` | `#2B2724` | Testo body |

### Font
- **Inter** (body) — Google Fonts, weight 400/500/600
- **Lora** (headings) — Google Fonts, weight 600/700

## 📄 Struttura File

```
Lisa_demo/
├── index.html           # Unico file: HTML + CSS + JS inline
├── .gitignore           # .DS_Store
├── .github/
│   └── workflows/       # (vuoto — deploy automatico di GitHub Pages)
└── README.md
```

## 🧩 Sezioni (14 pannelli)

| # | ID | Contenuto | Illustrazione |
|---|---|---|---|
| 1 | Hero | Logo Lisa, tagline, scroll cue | Ritratto Lisa + halo animato |
| 2 | Il problema | 68% anziani soli | ✅ Persona sola (SVG) |
| 3 | Cos'è Lisa | Una presenza, non un'app | ✅ Volto + chat bubble (SVG) |
| 4 | Su misura | Avatar multi-persona | Avatar colorati (CSS) |
| 5 | Come funziona | 4 passi | Emoji numerati |
| 6 | Sempre attenta | Voce, corpo, ambiente | Icone SVG rosa |
| 7 | Non dimentica | Medicine, visite, videochiamate | Emoji numerati |
| 8 | Solo compagnia | TV, chiacchiere, curiosità | ✅ TV + persona (SVG) |
| 9 | Come comunica | Anziano, famiglia, medico | Emoji numerati |
| 10 | Perché è diversa | Memoria, privacy | ✅ Scudo + cuore (SVG) |
| 11 | Numeri | 14.1M over 65, 800K famiglie | Nessuna |
| 12 | Quando arriva | Timeline pilota | Nessuna |
| 13 | Chiusura | Parliamone + contatti | ✅ Ritratto Lisa (copia hero) |

## 🎯 UI/UX — Ottimizzazioni per anziani

- **Font ingranditi**: body 17-22px, heading 32-52px
- **Toggle Aa**: bottone in alto a destra, raddoppia i font
- **Contrasto 4.5:1+**: grigio scurito a `#4A4440`
- **Scroll-snap**: navigazione a pannelli con dots laterali + frecce
- **Nessuna animazione**: halo e bob disattivati
- **Google Fonts**: Inter + Lora (più leggibili di Arial/Georgia)

## 🚀 Comandi

```bash
# Clona il repo
git clone git@github.com:euroteamintadv/Lisa_demo.git
cd Lisa_demo

# Modifica diretta — è un singolo file HTML
open index.html    # Apri nel browser
code index.html    # Modifica con VS Code

# Push e deploy automatico
git add -A
git commit -m "messaggio"
git push
# Live in ~30 secondi su mylisa.net
```

## 🌐 DNS — Namecheap

| Type | Host | Value |
|---|---|---|
| A Record | @ | 185.199.108.153 |
| A Record | @ | 185.199.109.153 |
| A Record | @ | 185.199.110.153 |
| A Record | @ | 185.199.111.153 |
| CNAME | www | euroteamintadv.github.io |

## ⚙️ GitHub Pages Settings

👉 https://github.com/euroteamintadv/Lisa_demo/settings/pages

- **Source**: Deploy from a branch
- **Branch**: `main` → `/ (root)`
- **Custom domain**: `mylisa.net`
- **Enforce HTTPS**: ✅ ON

## 👤 Contatti

- **Alberto Finelli** — neuraccent.com
- **powered by Neuraccent Bucarest**

## 📝 Note

- L'immagine del ritratto Lisa è inline base64 (~145KB)
- Le illustrazioni SVG sono inline nel CSS/HTML
- Non ci sono dipendenze npm, build step, o framework
- Il file HTML è ~320KB (principalmente per il base64)
- Per modificare le illustrazioni SVG: cercare `<svg` nel file
- Per modificare la foto: cercare `data:image/jpeg;base64` e sostituire
