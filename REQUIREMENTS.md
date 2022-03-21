# Documentação de Requisitos

## Especificação
  - [PDF](./assets/especification.pdf)

## Protótipo
  - [Figma](https://www.figma.com/file/4sI0IP4YRbJTMOepIR8XaY/Prot%C3%B3tipo?node-id=0%3A1)

## Requisitos:

### Épicos:

|Num | Épico | Personas envolvidas | Descrição do épico |
| - | --------- | --------- | --------- |
|01 | Gerenciamento de usuários |Professor | Permitir que o professor realize o cadastro de novos professores na plataforma, visualize os usuários cadastrados, edite suas informações e realize a inativação do usuário.
|02 | Realizar login da aplicação | Professor, visitante | Diponibilizar interface de login para permitir que o professor realize o login na aplicação e permitir redefinição de senha.
|03 | Gerenciar conteúdo | Professor, visitante | Permitir que o professor realize o cadastro das disciplinas e seus respectivos conteúdos programáticos, edite suas informações e realize a inativação de uma disciplina. Permitir a visualização pública das informações das disciplinas cadastradas através do sistema ou importadas via Crawlers e seu conteúdo programático, bem como sua exportação para formato específico.

### Histórias de usuário

| E01US01 | Cadastro de usuário |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero cadastrar um novo professor no sistema, para que ele possa fazer a gestão das disciplinas |
|*Critérios de aceitação*|

| E01US02 | Editar informações do professor |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero editar as informações de um professor, para atualizar seu e-mail ou inativá-lo na aplicação|
|*Critérios de aceitação*|

| E01US03 | Listar professores |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero visualizar as informações dos professores cadastrados, para que eu possa realizar editar suas informações e inativá-lo|
|*Critérios de aceitação*|

| E01US03 | Listar professores |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero inativar o cadastro de outro professor, para que o mesmo não tenha mais acesso ao sistema|
|*Critérios de aceitação*|

| E02US01 | Realizar login |
|---------|-----------------|
| *Descrição da história* |  Como um visitante no sistema, quero realizar o login na aplicação, para que eu possa realizar operações no sistema|
|*Critérios de aceitação*|

| E02US02 | Redefinir senha |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero solicitar meu reset de senha, para que eu possa acessar novamente a aplicação|
|*Critérios de aceitação*|

| E03US01 | Cadastrar conteúdo programático |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero cadastrar conteúdos programáticos das disciplinas, para que ela fique disponível para acesso externo|
|*Critérios de aceitação*|

| E03US01 | Cadastrar conteúdo programático |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero visualizar a lista de disciplinas cadastradas, para que ela fique disponível para acesso externo|
|*Critérios de aceitação*|

| E03US01 | Cadastrar conteúdo programático |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero visualizar a lista de disciplinas cadastradas, para que ela fique disponível para acesso externo|
|*Critérios de aceitação*|


|  `R3 - Create de Conteúdo` |  Conteúdos Programáticos serão primeiramente carregados pelo web crawler, mas poderão ser criados por usuários da secretaria. |
|  `R4 - Update de Conteúdo` |  Conteúdos Programáticos poderão sofrer update. |
|  `R5 - Listagem de Disciplinas` |  Disciplinas serão listadas. |
|  `R6 - Busca de Disciplinas` |  Disciplinas poderão ser buscadas diretamente pelo seu código ou nome. Ao acessar a página da disciplina, será possível visualizar informações básicas sobre ela. |
|  `R7 - Export de Informações` |  Para cada disciplina será possível realizar a exportação de um relatório em PDF, trazendo detalhes mais ricos a respeito de sua ementa e conteúdos programáticos. |
|  `R8 - Log de Atividades` | Todas as alterações realizadas no sistema em produção ficarão registradas em uma tabela, guardando o ID do usuário, a data, o objeto modificado e o IP de acesso. |
