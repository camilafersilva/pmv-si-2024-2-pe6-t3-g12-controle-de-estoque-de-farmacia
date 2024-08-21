# Introdução

Texto descritivo com a visão geral do projeto abordado. Inclui o contexto, o problema, os objetivos, a justificativa e o público-alvo do projeto.

## Problema
Nesse momento você deve apresentar o problema que a sua aplicação deve  resolver. No entanto, não é a hora de comentar sobre a aplicação.

Descreva também o contexto em que essa aplicação será usada, se  houver: empresa, tecnologias, etc. Novamente, descreva apenas o que de  fato existir, pois ainda não é a hora de apresentar requisitos  detalhados ou projetos.

Nesse momento, o grupo pode optar por fazer uso  de ferramentas como Design Thinking, que permite um olhar de ponta a ponta para o problema.

> **Links Úteis**:
> - [Objetivos, Problema de pesquisa e Justificativa](https://medium.com/@versioparole/objetivos-problema-de-pesquisa-e-justificativa-c98c8233b9c3)
> - [Matriz Certezas, Suposições e Dúvidas](https://medium.com/educa%C3%A7%C3%A3o-fora-da-caixa/matriz-certezas-suposi%C3%A7%C3%B5es-e-d%C3%BAvidas-fa2263633655)
> - [Brainstorming](https://www.euax.com.br/2018/09/brainstorming/)

## Objetivos

Aqui você deve descrever os objetivos do trabalho indicando que o objetivo geral é desenvolver um software para solucionar o problema apresentado acima. 

Apresente também alguns (pelo menos 2) objetivos específicos dependendo de onde você vai querer concentrar a sua prática investigativa, ou como você vai aprofundar no seu trabalho.
 
> **Links Úteis**:
> - [Objetivo geral e objetivo específico: como fazer e quais verbos utilizar](https://blog.mettzer.com/diferenca-entre-objetivo-geral-e-objetivo-especifico/)

## Justificativa

Descreva a importância ou a motivação para trabalhar com esta aplicação que você escolheu. Indique as razões pelas quais você escolheu seus objetivos específicos ou as razões para aprofundar em certos aspectos do software.

O grupo de trabalho pode fazer uso de questionários, entrevistas e dados estatísticos, que podem ser apresentados, com o objetivo de esclarecer detalhes do problema que será abordado pelo grupo.

> **Links Úteis**:
> - [Como montar a justificativa](https://guiadamonografia.com.br/como-montar-justificativa-do-tcc/)

## Público-Alvo

Descreva quem serão as pessoas que usarão a sua aplicação indicando os diferentes perfis. O objetivo aqui não é definir quem serão os clientes ou quais serão os papéis dos usuários na aplicação. A ideia é, dentro do possível, conhecer um pouco mais sobre o perfil dos usuários: conhecimentos prévios, relação com a tecnologia, relações
hierárquicas, etc.

Adicione informações sobre o público-alvo por meio de uma descrição textual, diagramas de personas e mapa de stakeholders.

> **Links Úteis**:
> - [Público-alvo](https://blog.hotmart.com/pt-br/publico-alvo/)
> - [Como definir o público alvo](https://exame.com/pme/5-dicas-essenciais-para-definir-o-publico-alvo-do-seu-negocio/)
> - [Público-alvo: o que é, tipos, como definir seu público e exemplos](https://klickpages.com.br/blog/publico-alvo-o-que-e/)
> - [Qual a diferença entre público-alvo e persona?](https://rockcontent.com/blog/diferenca-publico-alvo-e-persona/)

# Especificações do Projeto

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade de requisitos, aplicar uma técnica de priorização de requisitos e detalhar como a técnica foi aplicada.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir que o usuário cadastre tarefas | ALTA | 
|RF-002| Emitir um relatório de tarefas no mês   | MÉDIA |

### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deve ser responsivo para rodar em um dispositivos móvel | MÉDIA | 
|RNF-002| Deve processar requisições do usuário em no máximo 3s |  BAIXA | 

Com base nas Histórias de Usuário, enumere os requisitos da sua solução. Classifique esses requisitos em dois grupos:

- [Requisitos Funcionais
 (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
 correspondem a uma funcionalidade que deve estar presente na
  plataforma (ex: cadastro de usuário).
- [Requisitos Não Funcionais
  (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
  correspondem a uma característica técnica, seja de usabilidade,
  desempenho, confiabilidade, segurança ou outro (ex: suporte a
  dispositivos iOS e Android).
Lembre-se que cada requisito deve corresponder à uma e somente uma
característica alvo da sua solução. Além disso, certifique-se de que
todos os aspectos capturados nas Histórias de Usuário foram cobertos.

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre |
|02| Não pode ser desenvolvido um módulo de backend        |

Enumere as restrições à sua solução. Lembre-se de que as restrições geralmente limitam a solução candidata.

> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

# Catálogo de Serviços

Descreva aqui todos os serviços que serão disponibilizados pelo seu projeto, detalhando suas características e funcionalidades.

# Arquitetura da Solução


## 1. Definição dos Componentes

- **Interface Web**: Onde o usuário interage com o sistema.
- **API Gateway**: Ponto de entrada para todas as requisições, responsável por autenticação, autorização e roteamento.
- **Microsserviço "Produto"**: Gerencia as operações relacionadas aos medicamentos.
- **Banco de Dados (SQL Server)**: Armazena os dados dos medicamentos.
- **RabbitMQ**: Sistema para comunicação assíncrona entre microsserviços.
- **Microsserviço "Relatórios"**: Atualiza e gera relatórios de estoque.

## 2. Fluxo de Interação

### 2.1 Criar um Novo Medicamento

1. O usuário (Admin) insere os dados de um novo medicamento na interface web.
2. A interface web envia uma requisição HTTP POST para a API Gateway com os dados do novo medicamento.
3. A API Gateway valida a autenticação do usuário e verifica as permissões.
4. A API Gateway roteia a requisição para o microsserviço “Produto”.
5. O microsserviço “Produto” recebe a requisição, valida os dados e insere o novo medicamento no banco de dados (SQL Server).
6. Após a inserção, o microsserviço “Produto” envia uma mensagem para o RabbitMQ informando a criação do novo medicamento.
7. O microsserviço “Relatórios” recebe a mensagem e atualiza os relatórios de estoque.
8. O microsserviço “Produto” retorna uma resposta HTTP 201 (Created) para a API Gateway.
9. A API Gateway repassa a resposta para a interface web.
10. A interface web exibe uma mensagem de sucesso para o usuário.

### 2.2 Ler um Medicamento

1. O usuário (Admin) solicita a visualização dos dados de um medicamento na interface web.
2. A interface web envia uma requisição HTTP GET para a API Gateway.
3. A API Gateway valida a autenticação do usuário e verifica as permissões.
4. A API Gateway roteia a requisição para o microsserviço “Produto”.
5. O microsserviço “Produto” consulta o banco de dados (SQL Server) e retorna os dados do medicamento.
6. O microsserviço “Produto” retorna uma resposta HTTP 200 (OK) com os dados do medicamento para a API Gateway.
7. A API Gateway repassa a resposta para a interface web.
8. A interface web exibe os dados do medicamento para o usuário.

### 2.3 Atualizar um Medicamento

1. O usuário (Admin) edita os dados de um medicamento na interface web.
2. A interface web envia uma requisição HTTP PUT para a API Gateway com os dados atualizados.
3. A API Gateway valida a autenticação do usuário e verifica as permissões.
4. A API Gateway roteia a requisição para o microsserviço “Produto”.
5. O microsserviço “Produto” recebe a requisição, valida os dados e atualiza o medicamento no banco de dados (SQL Server).
6. Após a atualização, o microsserviço “Produto” envia uma mensagem para o RabbitMQ informando a atualização do medicamento.
7. O microsserviço “Relatórios” recebe a mensagem e atualiza os relatórios de estoque.
8. O microsserviço “Produto” retorna uma resposta HTTP 200 (OK) para a API Gateway.
9. A API Gateway repassa a resposta para a interface web.
10. A interface web exibe uma mensagem de sucesso para o usuário.

### 2.4 Excluir um Medicamento

1. O usuário (Admin) solicita a exclusão de um medicamento na interface web.
2. A interface web envia uma requisição HTTP DELETE para a API Gateway.
3. A API Gateway valida a autenticação do usuário e verifica as permissões.
4. A API Gateway roteia a requisição para o microsserviço “Produto”.
5. O microsserviço “Produto” recebe a requisição e remove o medicamento do banco de dados (SQL Server).
6. Após a exclusão, o microsserviço “Produto” envia uma mensagem para o RabbitMQ informando a exclusão do medicamento.
7. O microsserviço “Relatórios” recebe a mensagem e atualiza os relatórios de estoque.
8. O microsserviço “Produto” retorna uma resposta HTTP 200 (OK) para a API Gateway.
9. A API Gateway repassa a resposta para a interface web.
10. A interface web exibe uma mensagem de sucesso para o usuário.

### 3. Atualização do Banco de Dados

1. O microsserviço "Produto" recebe a requisição.
2. O microsserviço "Produto" valida os dados.
3. O microsserviço "Produto" atualiza o medicamento no banco de dados (SQL Server).

### 4. Notificação de Atualização

1. Após a atualização, o microsserviço "Produto" envia uma mensagem para o RabbitMQ informando a atualização.

### 5. Atualização de Relatórios

1. O microsserviço "Relatórios", subscrito na fila do RabbitMQ, recebe a mensagem.
2. O microsserviço "Relatórios" atualiza os relatórios de estoque em background.

### 6. Confirmação da Operação

1. O microsserviço "Produto" retorna uma resposta HTTP 200 (OK) para a API Gateway.
2. A API Gateway repassa a resposta para a interface web.
3. A interface web exibe uma mensagem de sucesso para o usuário.

<!-- ![arq](https://github.com/user-attachments/assets/b9402e05-8445-47c3-9d47-f11696e38a3d) -->

## Tecnologias Utilizadas

- Linguagem de Programação: C# (Backend) / HTML, CSS, JS (Frontend).
- Framework Backend: ASP.NET Core (para criação de APIs RESTful).
- Framework Frontend: React (para interface web responsiva) / React Native (para aplicativo móvel).
- Banco de Dados: SQL Server (confiabilidade e robustez).
- Cache: Redis (armazenamento em memória para alta performance).
- Message Broker: RabbitMQ (comunicação assíncrona e escalabilidade).
- IDEs: Visual Studio, Visual Studio Code.
- Ferramentas: Git (controle de versão), Swagger (documentação da API).

| Passo | Ação | Detalhes |
|---|---|---|
| 1 | Usuário interage com o sistema | Acessa o sistema via Navegador/Aplicativo. |
| 2 | Requisição enviada para a API | O Navegador/Aplicativo envia a requisição para a API (ASP.NET Core). |
| 3 | Verificação no Cache | A API verifica se os dados solicitados estão presentes no Cache (Redis). |
| 4 | Dados em Cache (Cache Hit) | Se os dados estiverem no cache: <br> - A API recupera os dados do Cache. <br> - A API retorna os dados para o Navegador/Aplicativo. |
| 5 | Dados não encontrados no Cache (Cache Miss) | Se os dados não estiverem no cache: <br> - A API publica uma mensagem na fila (RabbitMQ). |
| 6 | Microserviço processa a mensagem | O Microserviço (C#) consome a mensagem da fila. |
| 7 | Consulta ao Banco de Dados | O Microserviço consulta o Banco de Dados (SQL Server) pelos dados. |
| 8 | Retorno dos dados | O Microserviço retorna os dados para a fila (RabbitMQ). |
| 9 | API processa os dados | A API consome a mensagem da fila com os dados. | 
| 10 | Armazenamento em Cache | A API armazena os dados no Cache (Redis) para futuras requisições. |
| 11 | Retorno para o Usuário | A API retorna os dados para o Navegador/Aplicativo, que os exibe para o Usuário. |

## Hospedagem

Explique como a hospedagem e o lançamento da plataforma foi feita.

> **Links Úteis**:
>
> - [Website com GitHub Pages](https://pages.github.com/)
> - [Programação colaborativa com Repl.it](https://repl.it/)
> - [Getting Started with Heroku](https://devcenter.heroku.com/start)
> - [Publicando Seu Site No Heroku](http://pythonclub.com.br/publicando-seu-hello-world-no-heroku.html)
