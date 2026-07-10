# Trabalho de Conclusão da Disciplina – Integração Contínua com GitHub Actions

# Objetivo
Desenvolver uma pipeline de integração contínua utilizando GitHub Actions para um projeto com testes automatizados, contemplando:

Execução por push;
Execução manual;
Execução agendada (schedule);
Geração de relatório de testes;
Armazenamento/publicação do relatório na pipeline;
Criação de documentação explicando a solução e os conceitos utilizados.

## Requisitos
- Trabalho individual;
- Utilização do GitHub Actions;
- Pipeline executando com sucesso;
- Testes automatizados executando com sucesso;
- Relatórios gerados e armazenados na pipeline;
- Aplicação dos conceitos de Integração Contínua;
- Uso adequado das ferramentas propostas;
- Documentação completa através deste README.

## Tecnologias Utilizadas
- Node.js
- JavaScript (ES Modules)
- Git
- GitHub
- GitHub Actions
- Mocha
- ESLint
- Mochawesome

## Instalação
1. Instale o [git](https://git-scm.com)
2. Instale o [nodejs](https://nodejs.org/)
3. Instale o Yarn - `npm install -g yarn`
4. Faça um clone do projeto:
   `git clone https://github.com/WilsonMourao/trab_conc_integracao_continua_pgats03.git`
5. Acessar o ficheiro do projeto:
   `cd trab_conc_integracao_continua_pgats03`
6. Instale as dependências
   ```npm install
      npm install -g yarn
      yarn
   ```
7. Execute os testes 
   `yarn run test
   `
8. Abra o relatório de execução dos testes em `reports`

## Testes Automatizados
Os testes automatizados foram implementados utilizando Mocha e Chai.

Os cenários de teste garantem a validação das regras de negócio da aplicação, permitindo identificar falhas automaticamente antes da publicação de alterações.

A execução dos testes ocorre:

- Localmente pelo desenvolvedor;
- Automaticamente pela pipeline do GitHub Actions.

## Relatório dos Testes
O projeto utiliza o Mochawesome para geração de relatórios detalhados dos testes executados.

Após a execução:
``yarn run test
``

Os relatórios são gerados na pasta:
``/reports
``
Os relatórios apresentam:

* Quantidade de testes executados;
* Testes aprovados;
* Testes reprovados;
* Tempo de execução;
* Detalhamento dos cenários executados.

## Pipeline de Integração Contínua

A pipeline foi implementada utilizando GitHub Actions.

Ela é executada automaticamente através dos seguintes gatilhos:

 - Push na branch main;
 - Execução manual (workflow_dispatch);
 - Execução agendada (schedule).

## Execução Manual da Pipeline
Para executar a pipeline manualmente:

* Acesse a aba Actions do GitHub;
* Selecione a workflow da pipeline;
* Clique em Run workflow;
* Escolha a branch desejada;
* Clique novamente em Run workflow.
