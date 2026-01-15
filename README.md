# Francesco Salvatori - Fashion Designer Portfolio

Portfolio di moda interattivo minimalista con texture beige, fotografie in bianco e nero, e layout a doppia pagina come un magazine.

## 🎨 Caratteristiche

- **CV Page**: Pagina dedicata al curriculum con foto personale e biografia
- **Portfolio Gallery**: 6 progetti navigabili con animazioni fluide
- **Sistema di caricamento immagini**: Integrazione IndexedDB per sostituire immagini con salvataggio permanente
- **Traduzione EN/IT**: Sistema completo di traduzione automatica con toggle interattivo
- **Design responsivo**: Ottimizzato per desktop e mobile
- **Texture carta**: Stile minimalista con texture sottili che simulano le fibre della carta

## 📦 Tecnologie

- **React 18.3** con TypeScript
- **Vite 6.0** per build e development
- **Tailwind CSS v4** per lo styling
- **Motion** (Framer Motion) per le animazioni
- **Lucide React** per le icone
- **IndexedDB** per lo storage locale delle immagini

## 🚀 Installazione

### 1. Clona/Crea il progetto

```bash
mkdir francesco-salvatori-portfolio
cd francesco-salvatori-portfolio
```

### 2. Installa le dipendenze

```bash
npm install
```

### 3. Avvia il server di sviluppo

```bash
npm run dev
```

### 4. Build per produzione

```bash
npm run build
```

## 📁 Struttura del progetto

```
portfolio-francesco-salvatori/
├── index.html                          # Entry point HTML
├── main.tsx                            # Bootstrap React
├── vite.config.ts                      # Configurazione Vite
├── package.json                        # Dipendenze
├── App.tsx                             # Componente principale con routing
│
├── components/
│   ├── CVPage.tsx                      # Pagina CV con foto e biografia
│   ├── PortfolioPage.tsx               # Galleria progetti (6 progetti)
│   ├── ProjectDetail.tsx               # Dettaglio singolo progetto
│   ├── Navigation.tsx                  # Barra di navigazione
│   ├── LanguageToggle.tsx              # Toggle EN/IT responsive
│   ├── PortfolioSpread.tsx             # Layout spread magazine
│   │
│   ├── figma/
│   │   └── ImageWithFallback.tsx       # Componente per gestione immagini
│   │
│   └── ui/                             # Componenti shadcn/ui (42 componenti)
│
├── styles/
│   └── globals.css                     # Stili globali, texture carta, font
│
└── utils/
    ├── imageStorage.ts                 # IndexedDB per storage immagini
    └── languageContext.tsx             # Context per sistema traduzione EN/IT
```

## 🎯 Funzionalità principali

### Sistema di traduzione EN/IT
- Toggle interattivo in alto a destra in ogni pagina
- Traduzione automatica di tutti i testi (CV, progetti, UI)
- Salvataggio preferenza lingua in React Context

### Sistema di caricamento immagini
- Upload immagini personalizzate per ogni progetto
- Storage permanente con IndexedDB
- Persistenza dopo refresh della pagina
- Supporto per tutti e 6 i progetti della gallery

### Progetti nella Gallery
1. **Marcel** - Fashion Photography (20+ immagini)
2. **Fragments of Silence** - Editorial Campaign (8 immagini)
3. **Vertigine** - Print Design (6 pagine magazine)
4. **In the Making** - Behind the Scenes (6 immagini)
5. **The Essence** - Minimalist Collection (6 immagini)
6. **Prigionieri** - Print Design (scrolling verticale)

## 🛠️ Dipendenze principali

```json
{
  "dependencies": {
    "react": "^18.3.1",
    "react-dom": "^18.3.1",
    "motion": "^11.11.17",
    "lucide-react": "latest",
    "class-variance-authority": "latest",
    "clsx": "latest",
    "tailwind-merge": "latest"
  },
  "devDependencies": {
    "@vitejs/plugin-react": "^4.3.4",
    "vite": "^6.0.3",
    "@types/react": "^18.3.18",
    "@types/react-dom": "^18.3.5",
    "typescript": "^5.7.2",
    "tailwindcss": "^4.0.0",
    "autoprefixer": "^10.4.20",
    "postcss": "^8.4.49"
  }
}
```

## 🎨 Personalizzazione

### Modificare i contenuti del CV
Edita `/components/CVPage.tsx`:
- Nome, titolo, biografia
- Esperienze lavorative
- Skills e competenze

### Modificare i progetti
Edita `/components/PortfolioPage.tsx` e `/components/ProjectDetail.tsx`:
- Titoli e descrizioni progetti
- Immagini (o usa l'upload integrato)
- Categorie e metadati

### Modificare le traduzioni
Edita `/utils/languageContext.tsx`:
- Aggiungi nuove chiavi di traduzione
- Modifica testi esistenti in EN/IT

## 📱 Responsive Design

Il portfolio è completamente responsive:
- **Desktop**: Layout a doppia pagina tipo magazine
- **Tablet**: Layout adattivo
- **Mobile**: Layout ottimizzato con controlli touch

Il toggle EN/IT è stato ottimizzato per mobile:
- Dimensioni ridotte su schermi piccoli
- Posizionamento `right-4` per evitare tagli
- Font e padding ridotti per compattezza

## 🚀 Deploy

### Vercel (consigliato)
```bash
npm install -g vercel
vercel
```

### Netlify
```bash
npm run build
# Carica la cartella dist/
```

### GitHub Pages
```bash
npm run build
# Configura GitHub Actions per deploy automatico
```

## 📝 Note

- Le immagini importate da Figma usano lo schema `figma:asset/`
- Le immagini personalizzate vengono salvate in IndexedDB
- Il sistema supporta sia immagini raster (PNG, JPG) che vettoriali (SVG)
- I font utilizzati: Montserrat (sans-serif) e Lora (serif)

## 👨‍💻 Autore

**Francesco Salvatori**  
Fashion Designer - Roma, Italia  
Nato nel 2003

---

Creato con React, Tailwind CSS e Motion • © 2026
