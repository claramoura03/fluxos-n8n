# 📊 B3 - Maiores Altas e Baixas do IBOV com N8N

Este projeto apresenta um fluxo no N8N que consome a **API da B3** para retornar as **maiores altas e maiores baixas** do índice **IBOV** (Ibovespa), utilizando duas requisições HTTP.

🔧 Criado por **Clara Moura** como prática do curso _Curso Completo de N8N: Do Básico à Inteligência Artificial_, o projeto exemplifica como utilizar APIs públicas com N8N de forma clara e funcional.

---

## 🚀 Funcionalidade

O fluxo é dividido em duas etapas principais:

1. **Primeira requisição (GET):**
   - Acessa o site da B3 para obter informações gerais.
2. **Segunda requisição (GET):**
   - Consulta diretamente a API oficial:
     ```
     https://cotacao.b3.com.br/mds/api/v1/InstrumentPriceFluctuation/ibov
     ```
   - Essa chamada retorna os dados de **maiores altas** e **maiores baixas** do índice IBOV.

---

## 🧠 Estrutura do Fluxo no N8N

A imagem a seguir representa a estrutura do fluxo implementado:

![Estrutura do fluxo N8N](https://github.com/claramoura03/fluxos-n8n/blob/main/b3-cotacoes/fluxo-n8n-b3-altas-baixas.png?raw=true)

---

## ✅ Exemplo de Funcionamento

Após executar o fluxo, os dados são retornados com sucesso, conforme a imagem abaixo:

![Resultado do fluxo](https://github.com/claramoura03/fluxos-n8n/blob/main/b3-cotacoes/resultado-fluxo-n8n-b3.png?raw=true)

---

## 📂 Arquivos do Repositório

- `fluxo-b3-altas-baixas.json`: Fluxo completo do N8N exportado.
- `fluxo-n8n-b3-altas-baixas.png`: Estrutura visual do fluxo.
- `resultado-fluxo-n8n-b3.png`: Execução do fluxo com retorno da API.
- `README.md`: Documento explicativo completo.

---

## 📥 Como Usar

1. Baixe ou clone este repositório.
2. Acesse seu painel N8N.
3. Importe o arquivo `fluxo-b3-altas-baixas.json`.
4. Execute o fluxo.
5. Verifique o resultado no painel ou conecte a um nó adicional de saída, como Telegram ou Email.

---

## 👩‍💻 Autoria

Este projeto foi desenvolvido por **Clara Moura** com fins educacionais.

📌 Instagram: [@crm89](https://www.instagram.com/crm89)  
📂 Repositório: [GitHub - fluxos-n8n](https://github.com/claramoura03/fluxos-n8n)

---

## 🏁 Conclusão

Este é mais um passo prático no domínio de automações com N8N. Com apenas dois nós HTTP, é possível acessar e manipular dados em tempo real, reforçando como o N8N pode ser uma ferramenta poderosa para integrações com APIs públicas.

---
