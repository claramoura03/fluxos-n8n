# 🧩 Integração Notion + n8n – Automação de Blocos no Notion com Fluxo Manual

Este repositório contém um fluxo simples e funcional criado com o **n8n** para integração com o **Notion** via API oficial. O objetivo é demonstrar, de forma clara e prática, como utilizar o n8n para enviar informações automaticamente a uma página do Notion.

---

## 🚀 O que este fluxo faz?

Com apenas um clique no botão **“Testar fluxo”** dentro do n8n, o processo envia um novo **bloco de texto** para uma **página específica do Notion**.

A mensagem enviada como exemplo é:

> _"Olá, mundo! Deixe seu Like e se Inscreva no canal!"_

Esse conteúdo é adicionado como um **bloco do tipo parágrafo**, utilizando o nó `Append Block` da integração com o Notion.

Esse fluxo é útil como modelo inicial para testar automações simples e expandi-las futuramente com conteúdos dinâmicos.

---

## 🛠️ Tecnologias Utilizadas

- `n8n`: Plataforma open source de automações low-code.
- `Notion API`: Para conexão segura e oficial com páginas do Notion.
- `JSON`: Para estruturação do fluxo.
- `Token de Integração do Notion`: Chave necessária para autenticação na API.

---

## 📂 Estrutura do Repositório

