# API de Usuários (NestJS)

API simples com NodeJS + NestJS para armazenar usuários (nome e e-mail) em memória (sem banco de dados).

Integrantes do grupo: 

Andréia Macedo de Lima
Silvanio de Souza Aguiar Junior
Denis Lucas Donato
Gênilson Martins Moreira
Renildo da Silva Santos Junior


## Instalação

```bash
npm install
```

## Executar

```bash
npm run start:dev
```

A API sobe em `http://localhost:3000`.

## Endpoints

| Método | Rota         | Descrição                    | Body                              |
|--------|--------------|-------------------------------|------------------------------------|
| POST   | /users       | Cria um usuário               | `{ "nome": "...", "email": "..." }` |
| GET    | /users       | Lista todos os usuários       | -                                   |
| GET    | /users/:id   | Retorna um usuário pelo id    | -                                   |
| DELETE | /users/:id   | Remove um usuário pelo id     | -                                   |

## Exemplos (curl)

```bash
curl -X POST http://localhost:3000/users -H "Content-Type: application/json" -d "{\"nome\":\"Andreia\",\"email\":\"andreia@teste.com\"}"

curl http://localhost:3000/users

curl http://localhost:3000/users/1

curl -X DELETE http://localhost:3000/users/1
```
