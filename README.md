# Desafio GoStack: Conceitos de Typescript com Node e arquitetura de software
Projeto desenvolvido durante a Semana 2 do bootcamp GoStack onde, por meio de uma aplicação node.js com typescript, foram introduzidos e exercitados conceitos de arquitetura de software como:
    - _Separation of Concerns_ com a criação de services, repositories e models
    - _Dependency inversion_
    - _DTO_(Data transfer Object)

## ⚙ Pré-requisitos
Para a execução do projeto em seu ambiente local é necessário possuir instalado:

- NodeJS em sua versão LTS
> https://nodejs.org/en/

## 🛠 Guia de instalação
1. Faça download do projeto do github
2. Após ter feito download do projeto, acesse o diretorio raiz do mesmo via linha de comando
3. No terminal, execute o comando npm install para instalar as dependências do projeto (Caso você tenha o yarn instalado em sua máquina, execute apenas yarn para a instalação das dependencias)
4. Tendo finalizado o processo anterior, execute o comando npm run dev (ou yarn dev), para executar a API e a partir desse momento a API estará sendo executada de forma local na porta 5000

## 📩 Rotas disponíveis na API
* `POST / transactions`: A rota recebe `title`, `value` e `type` dentro do corpo da requisição, sendo type o tipo da transação, que deve ser `income` para entradas (depósitos) e `outcome` para saídas (retiradas). Ao cadastrar uma nova transação, ela deve ser armazenada dentro de um objeto com o seguinte formato :

>`{ "id": "uuid", "title": "Salário", "value": 3000, "type": "income" }`

* `GET / transactions`: Essa rota retorna uma listagem com todas as transações que você cadastrou até agora, junto com o valor de soma de entradas, retiradas e total de crédito.

## 📋 Comandos disponíveis
* dev:server: execução da API em ambiente local
* test: execução dos testes validando o desenvolvimento da api
* build: gera o bundler dos arquivos Typescript da aplicação

## 📙 Enunciado
Todo o desafio foi realizado baseado no enunciado:
> https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-fundamentos-nodejs
