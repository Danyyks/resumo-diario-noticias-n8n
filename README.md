# ☕ NewsBot: O Estagiário que Nunca Dorme (n8n + Gemini)

Sabe aquela montanha de abas abertas com notícias que você jura que vai ler, mas só fecham quando o Chrome trava? Pois é. Eu criei uma automação no n8n que faz o trabalho sujo por mim: lê, filtra, resume e me entrega tudo mastigadinho no Discord antes mesmo do meu primeiro café.

## 🚀 O que essa belezinha faz?

Todos os dias, pontualmente às 06:00 AM, o workflow acorda e:

- **Garimpa:** Vai atrás dos feeds RSS de tecnologia (como o dev.to).
- **Filtra:** Nada de spam! Ele pega apenas as 3 notícias mais quentes de cada fonte.
- **Refina:** Passa tudo pelo Google Gemini (IA), que atua como um editor rigoroso.
- **Resume:** Gera resumos de até 50 palavras por notícia (curto, grosso e útil).
- **Entrega:** Cospe um Markdown elegante direto no meu canal do Discord.

## 🛠️ Anatomia do Workflow

Para não dizer que é mágica, aqui estão as peças do quebra-cabeça:

- **Trigger:** Cron agendado para as 06h (porque o robô não precisa de despertador).
- **Agentes de Coleta:** Nós de RSS Read + Limit para manter o foco.
- **Cérebro (IA):** Basic LLM Chain usando o modelo do Gemini para entender o que é relevante de verdade.
- **Organização:** Nós de Merge, Split Out e Aggregate para que os dados não virem uma bagunça de JSON.
- **Mensageiro:** Nó do Discord para a entrega final.

## 🧠 Por que isso é legal?

- **Economia de neurônios:** Não preciso caçar notícia técnica em 50 sites diferentes.
- **Foco total:** Só recebo o que importa, sem o ruído das redes sociais.
- **Zero custo:** Feito com ferramentas acessíveis e muita lógica de automação.

> "Automação não é sobre preguiça, é sobre eficiência seletiva." — Eu, provavelmente, enquanto lia o resumo de hoje.

# redumo-diario-noticias-n8n
# redumo-diario-noticias-n8n
