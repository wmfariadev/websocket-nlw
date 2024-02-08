# Sistema de Votação NLW Rocketseat

Este projeto foi criado como parte do evento Next Level Week (NLW) da Rocketseat, com o objetivo de implementar um sistema de votação em tempo real. Ele utiliza uma API Node.js escrita em TypeScript, com o framework Fastify para a criação do servidor e validação de dados utilizando Zod. O sistema faz uso de bancos de dados PostgreSQL para o cadastro de enquetes e Redis para armazenar os votos.

## Tecnologias Utilizadas

- Node.js
- TypeScript
- Fastify
- Zod
- PostgreSQL
- Redis
- Prisma
- Docker
- WebSocket
- Pub/Sub

## Funcionalidades

- Cadastro de enquetes
- Votação em tempo real
- Atualização de votos em tempo real utilizando WebSocket e Pub/Sub
- Armazenamento seguro de dados utilizando PostgreSQL e Redis
- Utilização de ORM para interação com os bancos de dados através do Prisma

## Configuração

1. Clone o repositório: `git clone https://github.com/wmfarinha/websocket-nlw.git`
2. Navegue até o diretório do projeto: `cd websocket-nlw`
3. Instale as dependências: `npm install`
4. Para `.env` preencha as credenciais do PostgreSQL.
5. Execute o Docker Compose para inicializar os bancos de dados: `docker-compose up -d`
6. Execute as migrations do Prisma para criar as tabelas no PostgreSQL: `npx prisma migrate dev`
7. Inicie o servidor: `npm run dev`

## Estrutura do Projeto
```
websocket-nlw/
├── prisma/
│ └── migrations/
├── src/
│ ├── http/
│ │ ├── routes/
│ │ └── ws/
│ ├── lib/
│ └── utils/
├── .env
├── .gitignore
├── docker-compose.yml
├── package.json
├── README.md
└── tsconfig.json
```


**Desenvolvido por [William Faria](https://github.com/wmfarinha)**
