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

| E01US03 | Inativar professores |
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

| E03US01 | Cadastrar disciplinas/conteúdo programático |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero cadastrar conteúdos programáticos das disciplinas, para que ela fique disponível para acesso externo|
|*Critérios de aceitação*|

| E03US01 | Visualizar disciplinas |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero visualizar a lista de disciplinas cadastradas, para que ela fique disponível para acesso externo|
|*Critérios de aceitação*|


| E03US02 | Visualizar detalhes da disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor ou visitante, quero visualizar a lista de disciplinas cadastradas para que eu possa visualizar seus detalhes|
|*Critérios de aceitação*|

| E03US03 | Visualizar histórico de alterações da disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor ou visitante, quero visualizar as alterações no conteúdo de uma disciplina, para que eu possa acompanhar as mudanças do conteúdo programático|
|*Critérios de aceitação*|


| E03US04 | Atualizar informações  da disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero editar as informações de uma disciplina cadastrada para que seu conteúdo programático esteja de acordo a realidade da disciplina |
|*Critérios de aceitação*|

| E03US05 | Inativar disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero inativar uma disciplina para que a mesma não esteja mais disponível para visualização pública |
|*Critérios de aceitação*|

| E03US06 | Exportar conteúdo de disciplina |
|---------|-----------------|
| *Descrição da história* | Como um professor ou um visitante, quero exportar o conteúdo de uma disciplina, para obter suas informações em formato específico padronizado |
|*Critérios de aceitação*|

| E03US07 | Criar serviço de importação de disciplinas |
|---------|-----------------|
| *Descrição da história* | Implementação de Crawler para importar dados de disciplinas. |
|*Critérios de aceitação*|