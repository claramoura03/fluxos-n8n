# 🌐 Busca de Endereço via ViaCEP (CEP + Logradouro) – n8n

Este fluxo do **n8n** realiza uma consulta ao serviço **ViaCEP** com base em um CEP e logradouro informados, retornando dados completos do endereço.

Ideal para automatizações que envolvem:
- Verificação de endereços em cadastros
- Preenchimento automático de campos
- Integração com sistemas externos de validação de dados

---

## 📌 Visão Geral do Fluxo

Este fluxo executa duas requisições HTTP para a API do [ViaCEP](https://viacep.com.br):
- Uma busca por **CEP** diretamente
- Outra busca por **logradouro + UF + cidade**

Retorna os seguintes dados:
- Logradouro
- Bairro
- Cidade
- UF
- Complemento
- IBGE
- DDD
- etc.

---

## 📂 Estrutura dos nós usados

- **Manual Trigger**: Inicia o fluxo manualmente.
- **Set**: Define os dados de entrada (CEP, logradouro, cidade, UF).
- **HTTP Request**: Consulta a API ViaCEP com os parâmetros definidos.
- **Merge**: Junta as informações de diferentes chamadas (quando necessário).
- **Function ou Set final**: Formata o resultado para exibição ou integração.

---

## 🖼️ Captura de tela do fluxo

![Visualização do Fluxo](https://github.com/claramoura03/fluxos-n8n/blob/main/viacep-busca-endereco/fluxo-n8n-http-request-viacep.png?raw=true)

---

## 📥 Como usar

1. Acesse sua instância do **n8n**.
2. Clique em **Import** e selecione o arquivo JSON do fluxo.
3. Altere os campos do nó `Set` para simular suas entradas (CEP ou logradouro).
4. Clique em **Executar Fluxo** para testar.
5. O retorno virá estruturado no painel de execução.

---

## 🧪 Exemplo de Entrada (no Set)

```json
{
  "cep": "01001-000",
  "logradouro": "Praça da Sé",
  "cidade": "São Paulo",
  "uf": "SP"
}
