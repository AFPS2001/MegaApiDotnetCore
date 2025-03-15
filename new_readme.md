Aqui está a documentação para o projeto **MegaApiDotnetCore**:

---

# MegaApiDotnetCore Documentation

## Overview
MegaApiDotnetCore é uma API backend construída com **.NET Core 3.1** para fornecer dados em formato JSON sobre os "robôs" da série Mega Man. Este projeto utiliza **Entity Framework Core** e outras dependências modernas para gerenciamento de dados e resposta da API.

## Endpoints da API

1. **GET /api/v1/robots**  
   Retorna uma lista de todos os robôs.

2. **GET /api/v1/robots/{id}**  
   Retorna os detalhes de um robô específico pelo seu ID.

3. **POST /api/v1/robots**  
   Endpoint para criar uma nova entrada de robô.

## Tecnologias Usadas

- **Entity Framework Core**: ORM para gerenciamento de dados.
- **RESTful API Design**: Estrutura de endpoints claros e eficazes.
- **Injeção de Dependência**: Usada para promover desacoplamento e maior testabilidade.

## Dependências

- **Microsoft.EntityFrameworkCore**: 3.1.8
- **Microsoft.EntityFrameworkCore.SqlServer**: 3.1.8
- **Newtonsoft.Json**: 12.0.2

## Estrutura de Arquivos

```
src
├── Controllers        [Rotas de endpoints]
├── Models             [Modelos de banco de dados]
├── Services           [Regras de negócios]
├── Middlewares        [Funções intermediárias entre a solicitação HTTP e a resposta]
├── Database           [Estruturas relacionadas ao banco de dados]
│   ├── DTOs           [Modelos de entrada e visualização]
│   ├── EntityFramework [Arquivos relacionados ao ORM]
│   │   ├── Context    [Configurações do contexto Entity]
│   │   ├── Migrations [Migrações para atualização do banco de dados]
│   ├── Repositories   [Padrão de Repositório]
```

## Licença

Este software está licenciado sob os termos da licença **MIT**.

---

Essa documentação fornece uma visão geral do projeto, suas dependências e como utilizá-lo para acessar os dados dos robôs da série Mega Man.
