# Criando o projeto

`npm init -y`

criar pasta src e o arquivo server.ts

## extensões (Typescript, tsx para desenvolvimento em TY, TSUP para build para converter para JS para produção )

`npm i typescript @types/node tsx tsup -D`

## Para criar o arquivo tsconfig.json

`npx tsc --init`
e ja trocar o "target": "es2016" para "target": "ES2020"

## Fastify

`npm i fastify`
dividir o fastify em dois arquivos (criando o app.ts para dividi-lo junto com o server.ts)

## Criar o arquivo GitIgnore

.gitignore

## Configurar o NPM

.npmrc

## Configurar variaveis de ambiente

.env

## para carregar para o projeto o arquivo env

`npm i dotenv`
criar pasta env e o arquivo index.ts

## instalar o zod para fazer as validações das variaveis

`npm i zod`

## instalar eslint

`npm i eslint @rocketseat/eslint-config -D`

## banco de dados

`npm i prisma -D`

`npm i @prisma/client`

para fazer conexão
`npx prisma migrate dev`

rodar prisma ver o banco
`npx prisma studio`

## Docker

`docker run --name api-solid-pg -e POSTGRESQL_USERNAME=docker -e POSTGRESQL_PASSWORD=docker -e POSTGRESQL_DATABASE=apisolid -p 5432:5432 bitnami/postgresql`

### Para startar o banco no docker

`docker start api-solid-pg(nome do banco)`

para parar o container
`docker stop api-solid-pg(nome do banco)`

## biblioteca para fazer hashing de senhas

`npm i bcryptjs`

como não é uma biblioteca desenvolvida para typescript, então precisa instalar separadamente o
`npm i -D @types/bcryptjs`

## Parte de testes

### Vitest

`npm i vitest vite-tsconfig-paths -D`
