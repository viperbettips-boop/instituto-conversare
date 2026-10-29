# Pequeno Manual de Bolso Mental — página de vendas (Next.js)

Next.js 15 (App Router) + TypeScript. 15 idiomas, cada um com sua própria URL,
todos gerados como páginas estáticas no build.

| Idioma | URL | Idioma | URL |
|---|---|---|---|
| Português | `/` | Russo | `/ru/` |
| Inglês | `/en/` | Turco | `/tr/` |
| Espanhol | `/es/` | Japonês | `/ja/` |
| Francês | `/fr/` | Chinês | `/zh/` |
| Alemão | `/de/` | Coreano | `/ko/` |
| Italiano | `/it/` | Árabe (direita→esquerda) | `/ar/` |
| Holandês | `/nl/` | Hindi | `/hi/` |
| Polonês | `/pl/` | | |

## Antes de publicar — edite `lib/config.ts`
- `SITE_URL`: seu domínio final (usado no SEO e nas prévias de link).
- `CHECKOUT`: link de pagamento por idioma (ou só `pt` e `padrao`).
- `PRECOS`: os valores em € e US$ são **exemplos** — troque pelos reais.

## Rodar no computador
```bash
npm install
npm run dev      # abre em http://localhost:3000
```

## Publicar na Vercel
1. Suba esta pasta para um repositório no GitHub.
2. Na Vercel: **Add New → Project → Import** o repositório.
3. A Vercel detecta Next.js sozinha. Clique em **Deploy**.

## Onde mudar o quê
- Textos de todos os idiomas: `content/texts.json`
- Layout da página: `components/Landing.tsx`
- Cores e estilo: `app/globals.css`
- Imagens (capas, páginas, logo, foto): `public/assets/`
