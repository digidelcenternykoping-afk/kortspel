# Kortspel – Solitaire

Klassiskt Klondike-solitaire med egen grafik som fungerar med mus och touch,
på mobil och dator.

Spela: https://digidelcenternykoping-afk.github.io/kortspel/

- Inga cookies, ingen spårning och inga externa resurser (typsnitt, CDN m.m.).
- Inställningar, statistik och pågående spel sparas i webbläsarens
  `localStorage` **bara** om spelaren trycker på "Godkänn" i notisen. Det kan
  när som helst stängas av och raderas i menyn.
- Dra 1 eller dra 3 kort väljs i menyn.

## Publicering

Spelet är rena statiska filer utan byggsteg, så det kan ligga på både
GitHub Pages och Cloudflare Pages samtidigt.

- **GitHub Pages:** grenen `main`, mapp `/`.
- **Cloudflare Pages:** koppla repot under *Workers & Pages → Create → Pages →
  Connect to Git*. Framework preset: *None*, Build command: tomt,
  Build output directory: `/`. Varje push till `main` publiceras automatiskt.
  Filen `_headers` lägger till säkerhetshuvuden (används bara av Cloudflare).
