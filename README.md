# Assistente VG

Dashboard pessoal (PWA) pra agenda, finanças, cripto, lembretes e ideias, com assistente de IA integrado via API da Anthropic.

🔗 **App:** https://victorgiuliani.github.io/assistente/

## Stack
- HTML/CSS/JS puros num único arquivo, zero build
- PWA (instalável no iOS/Android)
- Persistência via `localStorage`
- IA: Claude Sonnet 4.6 com prompt caching + streaming + histórico multi-turn
- Markdown rendering via [marked.js](https://github.com/markedjs/marked)
- Tipografia: Inter

## Seções
- **Agenda** — compromissos com categorias e prioridades
- **Finanças** — faturas, gastos fixos, assinaturas, investimentos, cripto, milhas
- **Pessoal** — lembretes recorrentes e ideias
- **IA** — Q&A sobre todos os dados acima
- **Config** — import/export JSON, gestão de categorias

## IA
A aba IA usa a API da Anthropic direto do browser. Pra usar:

1. Pegue uma chave em https://console.anthropic.com
2. Cole no campo "Chave API Anthropic" da aba IA (fica salva no `localStorage`)
3. Pergunte qualquer coisa — ele tem contexto completo do seu dashboard

**Custo aproximado:** com Sonnet 4.6 + prompt caching, cada pergunta custa ~$0.001-0.003. Caching reduz ~90% do input em perguntas seguidas (janela de 5 min).

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
