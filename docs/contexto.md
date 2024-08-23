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

As tabelas a seguir apresentam os requisitos funcionais e não funcionais que definem o escopo do projeto de controle de estoque de medicamentos para farmácias. Cada requisito foi identificado com um ID único, acompanhado por uma descrição e uma prioridade atribuída.

Para determinar a prioridade dos requisitos, foi utilizada uma abordagem de classificação em três níveis:

**Alta:** Requisitos essenciais que são críticos para o funcionamento do sistema. Devem ser implementados na primeira versão do sistema, pois sua ausência comprometeria a funcionalidade principal.

**Média:** Requisitos importantes, mas que não são críticos para o funcionamento básico do sistema. Embora desejáveis, sua ausência não impede o uso do sistema, mas pode impactar a eficiência ou a experiência do usuário.

**Baixa:** Requisitos desejáveis que agregam valor, mas que podem ser adiados para versões futuras do sistema. Não são essenciais para o funcionamento inicial.

Essa classificação foi aplicada para garantir que os aspectos mais críticos do sistema sejam priorizados no desenvolvimento. As tabelas a seguir organizam os requisitos de acordo com essa priorização.

### Requisitos Funcionais

| ID    | Descrição do Requisito                                                                                                       | Prioridade |
|-------|------------------------------------------------------------------------------------------------------------------------------|------------|
| **RF01** | **Criar Novo Medicamento:** O usuário deve poder cadastrar novos medicamentos no sistema, inserindo dados como nome, princípio ativo, fabricante, data de validade, quantidade em estoque e preço. | **Alta**   |
| **RF02** | **Ler Medicamento:** O usuário deve poder consultar os dados de um medicamento específico, utilizando filtros como nome, princípio ativo ou código de barras. | **Alta**   |
| **RF03** | **Atualizar Medicamento:** O usuário deve poder atualizar os dados de um medicamento já cadastrado, como quantidade em estoque, preço e data de validade. | **Alta**   |
| **RF04** | **Excluir Medicamento:** O usuário deve poder remover um medicamento do sistema, caso ele não esteja mais disponível ou não seja mais vendido. | **Alta**  |
| **RF05** | **Interface Web:** O sistema deve ter uma interface web para acesso e gestão dos medicamentos. | **Alta**   |
| **RF06** | **Aplicativo Mobile:** O sistema deve contar com um aplicativo mobile para acesso e gestão dos medicamentos. | **Alta**   |
| **RF07** | **Controle de Acesso:** O sistema deve permitir que somente usuários autenticados possam acessar e gerenciar os medicamentos, com diferentes níveis de acesso (administrador, farmacêutico, etc.). | **Alta**   |
| **RF08** | **Histórico de Movimentações:** O sistema deve registrar um histórico de todas as operações realizadas, como criação, atualização e exclusão de medicamentos. | **Baixa**  |
| **RF09** | **Alerta de Validade:** O sistema deve notificar o usuário sobre medicamentos que estão próximos da data de validade. | **Média**  |
| **RF10** | **Relatórios:** O sistema deve gerar relatórios de estoque, incluindo medicamentos em falta, com baixa quantidade ou próximos da validade. | **Baixa**  |
| **RF11** | **Tela de Login/Cadastro:** O sistema deve exibir uma tela para login e cadastro de usuários, permitindo o acesso ao sistema de controle de estoque de medicamentos. | **Alta**   |
| **RF12** | **Seleção de Opção de Login/Cadastro:** O sistema deve exibir uma opção para o usuário selecionar entre login ou cadastro na plataforma. | **Alta**   |
| **RF13** | **Cadastro de Usuário:** O sistema deve permitir que o usuário final (farmacêuticos, administradores, etc.) se cadastre com dados como email, senha, telefone, CPF e número do registro profissional (CRF). | **Alta**   |
| **RF14** | **Login com Credenciais Existentes:** O sistema deve permitir que o usuário (funcionário ou administrador) entre com o seu email, senha. | **Alta**   |
| **RF15** | **Recuperação de Senha:** O sistema deve permitir a recuperação de senha para os usuários cadastrados, enviando um link de redefinição para o email registrado. | **Média**  |



### Requisitos não Funcionais



| ID    | Descrição do Requisito                                                                                                                                                     | Prioridade |
|-------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------|
| **RNF01** | **Desempenho:** O sistema deve ser capaz de suportar consultas e atualizações em tempo real, com um tempo de resposta inferior a 2 segundos para operações básicas. | **Alta**       |
| **RNF02** | **Segurança:** O sistema deve garantir a segurança através de criptografia de dados sensíveis e autenticação robusta. | **Alta**       |
| **RNF03** | **Escalabilidade:** O sistema deve ser escalável para suportar um aumento no número de usuários e medicamentos cadastrados, sem perda de desempenho. | **Média**      |
| **RNF04** | **Usabilidade:** A interface deve ser intuitiva e fácil de usar, permitindo que usuários com diferentes níveis de conhecimento tecnológico possam utilizar o sistema sem dificuldades. | **Alta**       |
| **RNF05** | **Compatibilidade:** O sistema deve ser compatível com os principais navegadores web (Chrome, Firefox, Edge, Safari) e dispositivos móveis (Android, iOS). | **Alta**       |
| **RNF06** | **Disponibilidade:** O sistema deve estar disponível para uso 24/7, com um tempo de inatividade planejado não superior a 1 hora por mês para manutenção. | **Alta**       |
| **RNF07** | **Manutenibilidade:** O sistema deve ser projetado para facilitar a manutenção e a atualização, com código limpo e documentação adequada. | **Alta**      |
| **RNF08** | **Backup:** O sistema deve realizar backups automáticos dos dados ao menos uma vez por dia, garantindo a recuperação em caso de falha. | **Alta**       |
| **RNF09** | **Tempo de Recuperação:** Em caso de falha, o sistema deve ser capaz de restaurar o serviço em até 1 hora. | **Alta**      |




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
|02| Deverá ser desenvolvido uma aplicação web       |
|03| Deverá ser desenvolvida uma aplicação mobile       |


Enumere as restrições à sua solução. Lembre-se de que as restrições geralmente limitam a solução candidata.

> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

# Catálogo de Serviços

|ID|Serviço|Descição|
|--|-------|--------|
|01|Control de acesso|Capacidade de autenticar usuários cadastrados, provendo acesso ao sistema de forma segura.|
|02|Gerenciamento de itens|Capacidade de cadastrar, editar e excluir itens da base de dados.|
|03|Gerenciamento de fluxo de itens|Capacidade de acompanhar e gerenciar o fluxo de movimentação de itens cadastrados.|
|04|Detalhamento de itens|Capacidade de exibir detalhes técnicos como descrição, quantidade e movimentação de itens específicos.|
|05|Atualização de listagem de itens|Capacidade de atualizar em tempo real a listagem de itens após modificação no banco de dados.|
|06|Notificação|Capacidade de notificar o usuário do sistema a respeito de criações, alterações ou exclusão de itens.|
|07|Filtros de pesquisa|Capacidade de filtrar pesquisa de itens de acordo com ID, Nome, Data de cadastro e Data de atualização do item.|

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
