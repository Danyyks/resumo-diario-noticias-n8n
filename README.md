# ☕ Resumo Diário de Notícias com n8n

Workflow em n8n que gera um resumo diário das notícias mais quentes do mundo da tecnologia e entrega tudo direto em um canal do Discord.

## O que ele faz?

Todos os dias, pontualmente às **06:00 AM**, o workflow entra em ação:

**Garimpa:** Busca feeds RSS de sites de tecnologia (como o dev.to).  
**Filtra:** Seleciona apenas as 3 notícias mais relevantes de cada fonte.  
**Refina:** Usa Google Gemini como editor para avaliar relevância.  
**Resume:** Gera resumo de até 50 palavras por notícia.  
**Entrega:** Envia tudo em um Markdown bem bonitão para o canal do Discord.

## Anatomia do Workflow

**Trigger:** Cron agendado para as 06h.  
**Coleta:** RSS + Limit.  
**Cérebro (IA):** Basic LLM Chain com Google Gemini.  
**Organização:** Merge, Split Out e Aggregate.  
**Entrega:** Nó do Discord.

## Por que isso é legal?

**Economia de tempo:** Nada de caçar notícias em vários sites.  
**Foco total:** Só recebo o que importa.  
**Zero custo:** Automação com ferramentas acessíveis.

## Requisitos

n8n (self-hosted ou cloud).  
Conta no Discord com webhook configurado.  
Api Key do Google Gemini.  
Fontes RSS configuradas.

## Como usar

1. Importe o workflow no seu n8n.
2. Configure as credenciais.  
   Discord e Google Gemini.
3. Ajuste os feeds RSS conforme suas preferências.
4. Ative o workflow!
