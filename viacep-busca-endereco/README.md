# 🔍 Fluxo n8n - Busca de Endereço via ViaCEP (CEP + Logradouro)

Este repositório contém um fluxo criado no **n8n** que realiza uma requisição à API pública do [ViaCEP](https://viacep.com.br/) para consultar endereços com base em um **CEP** e um **logradouro**.

---

## 📌 Objetivo

Automatizar a busca de dados de endereço no Brasil, combinando dois parâmetros:
- **CEP**: Código de Endereçamento Postal
- **Logradouro**: Nome da rua, avenida, etc.

Esse fluxo é útil para:
- Validar ou completar cadastros
- Automatizar formulários
- Enriquecer bases de dados

---

## ⚙️ Como funciona

📌 O fluxo está dividido em três blocos principais:

1. **Disparo manual** (`When clicking 'Test workflow'`):  
   Inicia o fluxo manualmente.

2. **HTTP Request (GET)** – Primeira requisição:  
   Consulta o **CEP** informado no endpoint da API do ViaCEP.

3. **HTTP Request (GET)** – Segunda requisição:  
   Consulta novamente o **CEP** para validar ou complementar com o **logradouro**.

---

## 🧩 Estrutura do fluxo (visual)

![Visualização do fluxo](https://github.com/claramoura03/fluxos-n8n/blob/main/viacep-busca-endereco/fluxo-n8n-http-request-viacep.png?raw=true)

---

## 📁 Arquivo incluído

| Nome do arquivo | Descrição |
|-----------------|-----------|
| `Busca de endereço via ViaCEP (CEP + Logradouro).json` | Exportação do fluxo em JSON para ser importado no n8n |

---

## 🛠️ Como importar no n8n

1. Abra o **n8n**.
2. Clique em **Import** (ícone de pasta).
3. Selecione o arquivo `Busca de endereço via ViaCEP (CEP + Logradouro).json`.
4. Clique em **Execute Workflow** ou use o botão **Test workflow**.

---

## 📦 API utilizada

- [ViaCEP - https://viacep.com.br/ws/](https://viacep.com.br/)
  - Gratuita, pública e sem necessidade de autenticação.
  - Limite razoável de requisições por minuto.

---

## 📌 Exemplo de resposta

```json
{
  "cep": "01001-000",
  "logradouro": "Praça da Sé",
  "complemento": "lado ímpar",
  "bairro": "Sé",
  "localidade": "São Paulo",
  "uf": "SP",
  "ibge": "3550308",
  "gia": "1004",
  "ddd": "11",
  "siafi": "7107"
}
