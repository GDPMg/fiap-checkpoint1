RM: 98694 / NOME: GUILHERME DAL POSOLO MATHEUS

RM: 97969 / NOME: GUSTAVO BRISQUI MARTINEZ

1- Criar um novo pedido.
![image](https://github.com/user-attachments/assets/b9b87d6f-551d-4a24-860f-9649361e332e)

2 - Buscar todos os pedidos
![image](https://github.com/user-attachments/assets/fc6d57e0-dd78-4f3e-a978-e3b683df5c6b)

3- Buscar um pedido pelo ID.
![image](https://github.com/user-attachments/assets/5f9ac6a5-f7e2-4bf3-bc0f-73ddaf5529c5)

4- Atualizar um pedido
![image](https://github.com/user-attachments/assets/b95b0611-ae3e-44ac-85e3-2d4a74c3f0e9)

5- Deletar um pedido.
![image](https://github.com/user-attachments/assets/cda58905-4912-4c3e-883c-0bf3f26f1a84)

Fazendo um GET novamente para mostrar que realmente deletou.
![image](https://github.com/user-attachments/assets/1feaabfc-b766-42ef-9d91-ca734fb5f2dd)

README:
# 📦 API de Pedidos

Esta API permite criar, consultar, atualizar e deletar pedidos. Abaixo estão listados os endpoints disponíveis, suas descrições e exemplos de uso.

---

## 📝 1. Criar um Novo Pedido

**Endpoint:**  
`POST /pedidos`

**Descrição:**  
Cria um novo pedido. O campo `dataPedido` é preenchido automaticamente com a data atual.

**Exemplo de Requisição:**

```json
{
  "clienteNome": "Fulano de Tal",
  "valorTotal": 150.0
}

{
  "id": 1,
  "clienteNome": "Fulano de Tal",
  "dataPedido": "2025-03-28",
  "valorTotal": 150.0
}


[
  {
    "id": 1,
    "clienteNome": "Fulano de Tal",
    "dataPedido": "2025-03-28",
    "valorTotal": 150.0
  },
  {
    "id": 2,
    "clienteNome": "Maria Silva",
    "dataPedido": "2025-03-28",
    "valorTotal": 250.0
  }
]

## 📋 2. Buscar Todos os Pedidos

### 🔗 Endpoint


### 📄 Descrição
Retorna uma lista com todos os pedidos cadastrados.

### 📦 Exemplo de Resposta
```json
[
  {
    "id": 1,
    "clienteNome": "Fulano de Tal",
    "dataPedido": "2025-03-28",
    "valorTotal": 150.0
  },
  {
    "id": 2,
    "clienteNome": "Maria Silva",
    "dataPedido": "2025-03-28",
    "valorTotal": 250.0
  }
]

## 🔎 3. Buscar um Pedido pelo ID

### 🔗 Endpoint


### 📄 Descrição
Retorna os detalhes de um pedido específico.

### 🚩 Exemplo de uso


### 📦 Exemplo de Resposta
```json
{
  "id": 1,
  "clienteNome": "Fulano de Tal",
  "dataPedido": "2025-03-28",
  "valorTotal": 150.0
}

## ✏️ 4. Atualizar um Pedido

### 🔗 Endpoint


### 📄 Descrição
Atualiza os dados de um pedido existente.

### 🚩 Exemplo de uso


### 📥 Exemplo de Requisição
```json
{
  "clienteNome": "Fulano Atualizado",
  "valorTotal": 200.0
}

Exemplo de Resposta

{
  "id": 1,
  "clienteNome": "Fulano Atualizado",
  "dataPedido": "2025-03-28",
  "valorTotal": 200.0
}

5. Deletar um Pedido
Endpoint:
DELETE /pedidos/{id}

Descrição:
Remove um pedido específico do banco de dados.
Exemplo: DELETE /pedidos/1

Resposta:

Status: 204 No Content em caso de sucesso.

Caso o ID informado não exista, a API retorna 404 Not


