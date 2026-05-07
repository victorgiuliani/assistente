# Assistente VG

Dashboard pessoal (PWA) pra agenda, finanças, cripto, lembretes e ideias, com assistente de IA integrado via API da Anthropic.

🔗 **App:** https://victorgiuliani.github.io/assistente/

## Stack
- HTML/CSS/JS puros num único arquivo, zero build
- PWA (instalável no iOS/Android)
- Persistência via `localStorage`
- Tipografia: Inter

## Seções
- **Agenda** — compromissos com categorias e prioridades
- **Finanças** — faturas, gastos fixos, assinaturas, investimentos, cripto, milhas
- **Pessoal** — lembretes recorrentes e ideias
- **Config** — import/export JSON, gestão de categorias

## Dev local
```bash
# qualquer servidor estático funciona
python -m http.server 8000
# ou
npx serve
```

Abra `http://localhost:8000`.

## Deploy
GitHub Pages — só fazer push pra `main`.
