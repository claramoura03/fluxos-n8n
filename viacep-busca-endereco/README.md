# Busca de Endereço via ViaCEP (CEP + Logradouro)

Este fluxo faz uso da API pública do [ViaCEP](https://viacep.com.br/) para buscar dados de endereço:

- A primeira requisição consulta diretamente um CEP.
- A segunda busca por logradouros com base em UF, cidade e nome da rua.

---

## 📌 Objetivo

Praticar requisições HTTP com o nó `HTTP Request` do n8n, aprendendo como usar parâmetros na URL e interpretar os retornos JSON de APIs públicas.

---

## ⚙️ Estrutura do Fluxo

![estrutura-do-fluxo](estrutura-do-fluxo.png)

---

## 🧪 Exemplos utilizados

1. **CEP direto**:  
   URL: `https://viacep.com.br/ws/01001000/json/`  
   Resultado: Endereço da Praça da Sé – São Paulo

2. **Busca por logradouro**:  
   URL: `https://viacep.com.br/ws/RS/Porto Alegre/Domingos/json/`  
   Resultado: Lista de logradouros que correspondem ao filtro

---

## ✅ Como usar

1. Baixe o arquivo JSON [busca-endereco-viacep.json](busca-endereco-viacep.json).
2. Importe no seu ambiente n8n.
3. Execute o fluxo e verifique os retornos de cada requisição.

---

## 📷 Resultado da requisição

![resultado-da-requisicao](resultado-da-requisicao.png)

---

## 🗂️ Arquivos

- `busca-endereco-viacep.json`: fluxo completo exportado do n8n.
- `estrutura-do-fluxo.png`: visão geral do fluxo.
- `resultado-da-requisicao.png`: resultado prático da execução.
