# API de Usuários - Spring Boot

Este projeto é uma API REST simples desenvolvida com **Spring Boot** para gerenciar usuários em memória, com suporte completo a operações **CRUD** (Create, Read, Update, Delete). Os dados são armazenados em um `Map<Long, User>`, sem uso de banco de dados.

## ✅ Funcionalidades

- Criar usuário (`POST /users`)
- Listar todos os usuários (`GET /users`)
- Atualizar usuário por ID (`PUT /users/{id}`)
- Remover usuário por ID (`DELETE /users/{id}`)

## 🚀 Como executar

1. Certifique-se de ter o **Java 17+** e **Maven** instalados.
2. Clone este repositório:
   ```bash
   git clone https://github.com/diefersonsilveira/api-usuarios-springboot.git
   ```

A aplicação ficará disponível em:  
📍 **http://localhost:8080**

---

## 📦 Estrutura do Projeto

```
src
├── main
│   ├── java
│   │   └── com.example.atvAPI
│   │       ├── model
│   │       │   └── User.java
│   │       ├── service
│   │       │   └── UserService.java
│   │       ├── controller
│   │       │   └── UserController.java
│   │       └── AtvApiApplication.java
│   └── resources
│       └── application.properties
```

---

## 🧪 Testes com Postman

Todos os endpoints da API foram **testados com o Postman**, garantindo seu funcionamento adequado. Abaixo exemplos de requisições:

### 🔹 Criar Usuário
**POST** `/users`  
```json
{
  "nome": "Maria",
  "idade": 28
}
```

### 🔹 Listar Usuários
**GET** `/users`

### 🔹 Atualizar Usuário
**PUT** `/users/1`  
```json
{
  "nome": "Maria Souza",
  "idade": 29
}
```

### 🔹 Deletar Usuário
**DELETE** `/users/1`

---

## 🛠 Tecnologias

- Java 17
- Spring Boot
- Maven
- Postman (para testes)

---