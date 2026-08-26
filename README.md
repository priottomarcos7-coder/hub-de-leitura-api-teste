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