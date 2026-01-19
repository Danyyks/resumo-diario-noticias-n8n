# ☕ Resumo Diário de Notícias com n8n

Criei um workflow no n8n que me entrega um resumo diário das notícias mais quentes do mundo da tecnologia, direto no meu canal do discord.

## 🚀 O que ele faz?

Todos os dias, pontualmente às 06:00 AM, o workflow acorda e:

**Garimpa:** Vai atrás dos feeds RSS de tecnologia (como o dev.to).
**Filtra:** Nada de spam! Ele pega apenas as 3 notícias mais quentes de cada fonte.
**Refina:** Passa tudo pelo Google Gemini (IA), que atua como um editor rigoroso.
**Resume:** Gera resumos de até 50 palavras por notícia (direto ao ponto).
**Entrega:** Envia um Markdown bonitão direto no meu canal do Discord com as notícias.

## 🛠️ Anatomia do Workflow

**Trigger:** Cron agendado para as 06h.
**Agentes de Coleta:** Nós de RSS Read + Limit para manter o foco.
**Cérebro (IA):** Basic LLM Chain usando o modelo do Gemini para entender o que é relevante de verdade.
**Organização:** Nós de Merge, Split Out e Aggregate para que os dados não virem uma bagunça de JSON.
**Mensageiro:** Nó do Discord para a entrega final.

## 🧠 Por que isso é legal?

**Economia de tempo:** Não preciso caçar notícia técnica em 50 sites diferentes.
**Foco total:** Só recebo o que importa.
**Zero custo:** Feito com ferramentas acessíveis e muita lógica de automação.

# resumo-diario-noticias-n8n
