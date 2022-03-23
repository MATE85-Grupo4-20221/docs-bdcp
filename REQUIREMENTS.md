# Documentação de Requisitos

## Requisitos:

### Épicos:

|Num | Épico | Personas envolvidas | Descrição do épico |
| - | --------- | --------- | --------- |
|01 | Gerenciamento de usuários |Professor | Permitir que o professor gere convite para que novos professores se cadastrem, visualize os usuários cadastrados e edite suas informações.
|02 | Realizar login da aplicação | Professor | Disponibilizar interface de login para permitir que o professor realize o login na aplicação e permitir a redefinição de sua senha.
|03 | Gerenciar conteúdo | Professor, visitante | Permitir que o professor realize o cadastro  disciplinas e seus respectivos conteúdos programáticos, edite e aprove a alteração de suas informações e realize a inativação de uma disciplina. Permitir a visualização pública das informações das disciplinas cadastradas através do sistema ou importadas via Crawler e seu conteúdo programático, bem como sua exportação para formato específico.

### Histórias de usuário

| E01US01 | Gerar convite de cadastro para um professor |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero gerar um link de convite, para que um professor possa realizar seu cadastro |
|*Critérios de aceitação*| _Cenário 01: Gerar link de convite_ <br> Dado que o professor esteja visualizando os professores cadastrados <br> Quando clicar no botão gerar convite <br> Então o sistema exibirá um link com o convite para aplicação <br> E permitirá que o mesmo copie a informação 

| E01US02 | Permitir o cadastro usuário a partir de convite |
|---------|-----------------|
| *Descrição da história* | Como um professor que recebeu um covite de cadastro na plataforma, quero me cadastrar na aplicação, para que eu possa realizar a gestão das informações das disciplinas.
|*Critérios de aceitação*| Dado que o usuário deseja se cadastrar na aplicação <br> Quando possuir um link válido <br> Então o sistema permitirá que o usuário informe o seu "Nome Completo", "E-mail", "Senha" e que o usuário confirme sua senha na opção "Confirmar senha" <br><br> Dado que o professor esteja se cadastrando com um novo usuário <br> Quando informar um e-mail já cadastrado <br> Então o sistema exibirá a mensagem: "Professor já cadastrado" <br> E cancelará a operação


| E01US03 | Editar informações do professor |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero editar as informações de um professor, para atualizar seu nome ou e-mail |
|*Critérios de aceitação*| _Cenário 01: Editar informações professor_ <br> Dado que o usuário esteja visualizando a lista de professores <br> Quando clicar na opção de editar a informação de um professor <br> Então o sistema exibirá as informações do "Nome Completo" e "E-mail institucional" <br> E permitirá que o mesmo edite as informações descritas. <br> <br> Dado que o usuário esteja editando as informações <br> Quando não preencher uma informação <br> Então o sistema exibirá a mensagem: [Nome do campo] é obrigatório <br> E não concluirá a operação. <br> <br> Dado que o professor esteja editando as informações de um usuário <br> Quando alterar a informação de e-mail <br> E este já pertença a outro usuário cadastrado <br>Então o sistema exibirá a mensagem: "E-mail já cadastrado"<br> E cancelará a operação <br> <br> Dado que o usuário esteja editando as informações <br> Quando salvar as informações com sucesso <br> Então o sistema concluirá a operação <br> E redirecionará o usuário para a interface de listagem.


| E01US04 | Listar professores |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero visualizar as informações dos professores cadastrados, para que eu possa visualizar suas informações|
|*Critérios de aceitação*| Dado que o usuário esteja logado na aplicação <br> Quando desejar visualizar a lista de professores <br> Então o sistema disponibilizará em formato de grade as colunas "Nome", "E-mail" e "Status" de cada usuário <br> E ordenará a listagem pelo nome do usuário <br> E disponibilizará as opções de editar. 


| E02US01 | Realizar login |
|---------|-----------------|
| *Descrição da história* |  Como um usuário no sistema, quero realizar o login na aplicação, para que eu possa realizar operações no sistema|
|*Critérios de aceitação*| _Cenário 01: Realizar login_ <br> Dado que o usuário esteja na interface de login <br> Quando digitar um e-mail e senha válidos <br> Então o sistema redirecionará o usuário para interface de listagem de disciplinas.<br><br> _Cenário 02: Informar erro no login_ <br> Dado que o usuário esteja na interface de login <br> Quando digitar um e-mail e senha inválidos <br> Então o sistema exibirá a mensagem "Usuário ou senha incorretos" <br> E cancelará a operação.

| E02US02 | Redefinir senha |
|---------|-----------------|
| *Descrição da história* |  Como um professor previamente cadastrado, quero solicitar o reset de minha senha, para que eu possa acessar novamente a aplicação|
|*Critérios de aceitação*| _Cenário 01: Esqueci minha senha_ <br>Dado que o usuário clique na opção esqueci minha senha <br> Quando informar um e-mail previamente cadastrado <br> Então o sistema enviará um e-mail com um link para redefinição de senha. <br> <br> _Cenário 02: Redefinição de senha"_ <br> Dado que o usuário acesse o link do e-mail <br> Quando informar uma senha válida no campo "Senha" e confirmá-la corretamente na opção "Confirmar senha" <br> Então o sistema alterará a senha do usuário na aplicação <br> E efetuará automaticamente seu login <br> E o redirecionará para interface de listagem de disciplinas.

| E03US01 | Cadastrar disciplinas/conteúdo programático |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero cadastrar conteúdos programáticos das disciplinas, para que ela fique disponível para aprovação e publicação para acesso externo|
|*Critérios de aceitação*| _Cenário 01 - Cadastro de conteúdo programático_ <br> Dado que o professor esteja visualizando a lista de disciplinas <br> Quando clicar na opção "Cadastrar nova disciplina" <br> Então o sistema deverá disponibilizar, em ordem, que o usuário preencha os campos "Código" e "Nome" da disciplina (obrigatórios) <br> E selecione dentre as Modalidades: "Disciplina","Atividade", "Estágio", "Atividade complementar" ou "Trabalho de conclusão de curso". <br> E selecione Disciplinas para o campo "Pré-requisito", caso necessário <br> E preencha a "Carga horária" da disciplina, distribuindo entre as opções: "Teórica", "Prática" e "Estágio"<br> E preencha o "Módulo" da disciplina <br> E preencha o "Semestre letivo de aplicação" <br> E preencha a "Ementa", "Objetivos", "Conteúdo programático", "Metodologia", "Avaliação da aprendizagem" e "Bibliografia" da disciplina


| E03US02 | Visualizar disciplinas |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero visualizar a lista de disciplinas cadastradas, para que ela fique disponível para acesso externo|
|*Critérios de aceitação*| _Cenário 01: Buscar disciplinas_ <br> Dado que o usuário esteja na interface de listagem de disciplinas <br> Quando digitar alguma informação no campo "Nome ou código da disciplina" <br> Então o sistema buscará em tempo real _(autocomplete)_ as disciplinas que estejam de acordo ao filtro <br> E exibirá na grade de disciplinas. <br><br>_Cenário 02: Listar disciplinas_ <br> Dado que o usuário tenha informado algum dado no campo de busca <br> Quando houverem disciplinas que se encaixam na informação buscada <br> Então o sistema exibirá o código e nome da disciplina <br> E permitirá o clique para visualização dos detalhes da disciplina.


| E03US03 | Visualizar detalhes da disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor ou visitante, quero visualizar a lista de disciplinas cadastradas para que eu possa visualizar seus detalhes|
|*Critérios de aceitação*| _Cenário 01: Visualizar detalhes da disciplina_<br> Dado que o visitante esteja visualizando a lista de disciplinas retornadas pela busca <br> Quando clicar em uma disciplina <br> Então o sistema exibirá os detalhes das disciplinas através dos campos "Departamento", "Carga horária total", "Semestre vigente", "Ementa" e "Conteúdo programático".



| E03US04 | Visualizar histórico de alterações da disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor ou visitante, quero visualizar as alterações no conteúdo de uma disciplina, para que eu possa acompanhar as mudanças do conteúdo programático|
|*Critérios de aceitação*| _Cenário 01: Visualizar histórico da disciplina_<br> Dado que o visitante esteja visualizando os detalhes da disciplina <br> Quando clicar no histórico <br> Então o sistema exibirá o histórico de alterações em ordem cronológica do mais recente para o mais antigo.


| E03US05 | Atualizar informações  da disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero editar as informações de uma disciplina cadastrada para que seu conteúdo programático esteja de acordo a realidade da disciplina |
|*Critérios de aceitação*| Dado que o professor clique na disciplina buscada <br> Então o sistema exibirá a interface de visualização dos dados <br> E permitirá que o usuário edite as informações.

| E03US06 | Inativar disciplina |
|---------|-----------------|
| *Descrição da história* |  Como um professor, quero inativar uma disciplina para que a mesma não esteja mais disponível para visualização pública |
|*Critérios de aceitação*| Dado que o professor esteja visualizando os detalhes da disciplina <br> Então o sistema exibirá uma opção de inativar a disciplina <br> E permitirá que o usuário salve a operação.

| E03US07 | Exportar conteúdo de disciplina |
|---------|-----------------|
| *Descrição da história* | Como um professor ou um visitante, quero exportar o conteúdo de uma disciplina, para obter suas informações em formato específico padronizado |
|*Critérios de aceitação*|

| E03US08 | Criar serviço de importação de disciplinas |
|---------|-----------------|
| *Descrição da história* | Implementação de Crawler para importar dados de disciplinas. |
|*Critérios de aceitação*| Implementar crawler para que as disciplinas estejam disponíveis inicialmente na aplicação.
