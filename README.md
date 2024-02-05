# User management

Este projeto visa oferecer um sistema de gerenciamento de usuários simples usando o Spring Boot e o Hibernate.
## Requisitos

- Java 11 ou superior
- Maven 3.6.0 ou superior

## Como usar

1. Clone este repositório:

```bash
git clone https://github.com/JamesonHenrique/springboot-restful-webservices.git
```

2. Abra o projeto em seu IDE

3. Compile e execute o projeto

4. Use um cliente REST como o Postman para testar os pontos de extremidade

## Pontos de extremidade

### Criando um novo usuário

POST http://localhost:8080/api/users

Corpo da solicitação:

```json
{
  "name": "John Doe",
  "email": "johndoe@example.com"
}
```

Resposta:

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "johndoe@example.com"
}
```

### Recuperando um usuário por ID

GET http://localhost:8080/api/users/1

Resposta:

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "johndoe@example.com"
}
```
### Recuperando todos os usuárioS

GET http://localhost:8080/api/users

Resposta:

```json
{
  "id": 1,
  "name": "John Doe",
  "email": "johndoe@example.com"
}
 {
  "id": 2,
  "firstName": "Pedro",
  "lastName": "Henrique",
  "email": "pedrohenrique@example.com"
    }
```
### Atualizando usuários

PUT http://localhost:8080/api/users

Corpo da solicitação:

```json
{
  "name": "John Husbon",
  "email": "johnhusbon@example.com"
}
```

Resposta:

```json
{
  "id": 1,
  "name": "John Husbon",
  "email": "johnhusbon@example.com"
}
```
### Deletando usuários

DELETE http://localhost:8080/api/users

Resposta:

```json
User Deleted


