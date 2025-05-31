# 🤖 Chatbot Telegram com n8n

Este fluxo utiliza o `Telegram Trigger` do n8n para criar um chatbot que responde a comandos como `/start`, `/ajuda` e envia mensagens automáticas com base nas opções escolhidas pelo usuário.

![Fluxo do chatbot no n8n](https://github.com/claramoura03/fluxos-n8n/blob/main/chatbot-telegram/estrutura-do-fluxo.png.png?raw=true)

---

## 🚀 Tecnologias
- n8n
- Bot do Telegram (via BotFather)
- Webhook

## 🔁 Como usar
1. Crie seu bot no Telegram via @BotFather.
2. Copie o token e insira no nó Telegram Trigger do n8n.
3. Configure os comandos e mensagens no fluxo.
4. Teste enviando `/start` no seu bot.

## 📁 Arquivo
- `chatbot-telegram.json`

## 📌 Observações
Este projeto foi desenvolvido como prática após assistir ao vídeo:  
[🔗 Automação com Chatbot no Telegram e n8n](https://www.youtube.com/watch?v=G_U0-UMD_9E)

![Bot funcionando](https://github.com/claramoura03/fluxos-n8n/blob/main/chatbot-telegram/bot-funcionando.png.png?raw=true)
