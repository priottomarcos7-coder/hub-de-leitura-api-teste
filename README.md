# Testes Automatizados de API REST — Hub de Leitura

## Objetivo

Projeto de testes automatizados de API REST para a aplicação Hub de Leitura, desenvolvido durante a formação em Engenharia de Qualidade de Software.

O objetivo é validar endpoints, códigos HTTP, propriedades das respostas e regras de negócio em cenários positivos e negativos.

## Tecnologias

- Cypress 15.11.0
- Cypress Plugin API
- JavaScript
- Node.js
- API REST

## Pré-requisitos

- Node.js instalado
- npm instalado
- Git
- API do Hub de Leitura disponível e configurada para os testes

## Instalação

Clone o repositório:

```bash
git clone https://github.com/priottomarcos7-coder/hub-de-leitura-api-teste.git
cd hub-de-leitura-api-teste
```

Instale as dependências:

```bash
npm install
```

## Execução dos testes

Como o `package.json` deste projeto não possui um script de teste configurado, execute o Cypress diretamente:

```bash
npx cypress run
```

Para abrir a interface do Cypress:

```bash
npx cypress open
```

## Cenários automatizados

Os testes incluem:

- GET para listar usuários
- GET de usuário por ID
- GET utilizando filtros e parâmetros
- Validação das propriedades dos usuários retornados
- POST para cadastro de usuário
- Validação de e-mail inválido
- PUT para atualização de usuário
- PUT com identificação dinâmica do usuário
- DELETE de usuário
- DELETE com identificação dinâmica

## Estratégia de testes

Foram utilizados cenários positivos e negativos, validação de códigos HTTP e validação do conteúdo das respostas. Também foram utilizados dados dinâmicos para reduzir dependência de registros fixos.

## Estrutura principal

```text
cypress/
└── e2e/
    └── usuarios.cy.js

cypress.config.js
package.json
```

## Resultado esperado

Os testes devem apresentar no Cypress o resultado de cada cenário, permitindo identificar respostas corretas, falhas e comportamentos que precisam de investigação.

## Repositório

https://github.com/priottomarcos7-coder/hub-de-leitura-api-teste

## Autor

Marcos Priotto

Projeto desenvolvido como parte da formação em Engenharia de Qualidade de Software na EBAC.
---

# English Version

# Automated REST API Tests — Reading Hub

## Goal

REST API test automation project for the Reading Hub application, developed during Software Quality Engineering training.

The goal is to validate endpoints, HTTP status codes, response properties, and business rules across positive and negative scenarios.

## Technologies

- Cypress 15.11.0
- Cypress API Plugin
- JavaScript
- Node.js
- REST API

## Prerequisites

- Node.js installed
- npm installed
- Git
- Reading Hub API available and configured for testing

## Installation

Clone the repository:

```bash
git clone https://github.com/priottomarcos7-coder/hub-de-leitura-api-teste.git
cd hub-de-leitura-api-teste
```

Install the dependencies:

```bash
npm install
```

## Running the Tests

Since this project's `package.json` does not define a test script, run Cypress directly:

```bash
npx cypress run
```

To open the Cypress UI:

```bash
npx cypress open
```

## Automated Scenarios

The tests include:

- GET to list users
- GET a user by ID
- GET using filters and parameters
- Validation of properties in returned user records
- POST to create a user
- Validation of an invalid email address
- PUT to update a user
- PUT using a dynamically obtained user ID
- DELETE a user
- DELETE using a dynamically obtained ID

## Testing Strategy

Positive and negative scenarios, HTTP status code validation, and response-content validation were used. Dynamic data was also used to reduce dependence on fixed records.

## Main Structure

```text
cypress/
└── e2e/
    └── usuarios.cy.js

cypress.config.js
package.json
```

## Expected Results

Cypress should display the result of each scenario, helping identify correct responses, failures, and behaviors that require further investigation.

## Repository

https://github.com/priottomarcos7-coder/hub-de-leitura-api-teste

## Author

Marcos Priotto

Project developed as part of the Software Quality Engineering training program at EBAC.
