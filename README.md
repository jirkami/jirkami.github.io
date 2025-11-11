# Michal Jirka - Portfolio

Portfolio website pro Ing. Michala Jirku - specialistu na systémovou správu a IT infrastrukturu.

## Technologie

- **Hugo** - Static site generator
- **Hugoplate Theme** - Moderní Hugo theme s Tailwind CSS
- **TailwindCSS 4** - Utility-first CSS framework
- **Dark Mode** - Primárně tmavý vzhled s modrými akcenty

## Instalace a spuštění

### Požadavky

- Hugo Extended (v0.144.0+)
- Node.js a npm
- Go (pro Hugo modules)

### Lokální vývoj

```bash
# Instalace závislostí
npm install

# Inicializace Hugo modules
hugo mod tidy

# Spuštění development serveru
hugo server -D

# Build pro produkci
hugo --cleanDestinationDir
```

## Struktura

```
.
├── config/               # Konfigurace Hugo
│   └── _default/
│       ├── languages.toml
│       ├── menus.cs.toml
│       ├── module.toml
│       └── params.toml
├── content/
│   └── czech/           # Český obsah
│       ├── _index.md    # Hlavní stránka
│       ├── about/       # O mně
│       ├── services/    # Služby
│       ├── experience/  # Zkušenosti
│       └── contact/     # Kontakt
├── data/
│   ├── theme.json       # Barevná schémata
│   └── social.json      # Sociální sítě
├── static/
│   └── images/          # Obrázky (logo atd.)
├── themes/
│   └── hugoplate/       # Theme (git submodule)
└── hugo.toml            # Hlavní konfigurace
```

## Konfigurace

### Barvy

Tmavý režim s modrými akcenty je nakonfigurován v `data/theme.json`:
- Primary color (dark mode): `#3b82f6` (modrá)
- Body background: `#0f172a` (tmavě modrá)
- Border color: `#1e293b`

### Logo

Logo je umístěno v `static/images/infracore_logo.svg` a je nakonfigurováno v `config/_default/params.toml`.

### Menu

Menu je definováno v `config/_default/menus.cs.toml` a obsahuje sekce:
- O mně
- Služby
- Zkušenosti
- Kontakt

## Deployment

Site je automaticky buildován a deployován na GitHub Pages při pushu do main větve.

## Kontakt

**Ing. Michal Jirka**
- Email: george@infracore.cz
- Telefon: +420 608 556 186
- LinkedIn: [linkedin.com/in/jirkami](https://linkedin.com/in/jirkami)

## License

© 2024 Michal Jirka - Infracore. Všechna práva vyhrazena.
