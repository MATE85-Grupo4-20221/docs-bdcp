# Documentação de Requisitos

- Título
  - Banco de Conteúdos Programáticos (BDCP)

- Escopo do Projeto
  - O objetivo desta aplicação é centralizar informações importantes a respeito de ementas e conteúdos programáticos de cada disciplina respectiva a cada curso ofertado pela Universidade Federal da Bahia.

- Requisitos 

| Requisito | Descrição |
| --------- | --------- |
|  `R1 - Cadastro de Usuário` | Usuários (funcionários da secretaria ???) poderão realizar login no sistema para realizar update dos conteúdos programáticos. |
|  `R2 - Login de Usuário` | Usuários (funcionários da secretaria ???) poderão realizar login no sistema para realizar update dos conteúdos programáticos. |
|  `R3 - Create de Conteúdo` |  Conteúdos Programáticos serão primeiramente carregados pelo web crawler, mas poderão ser criados por usuários da secretaria. |
|  `R4 - Update de Conteúdo` |  Conteúdos Programáticos poderão sofrer update. |
|  `R5 - Listagem de Disciplinas` |  Disciplinas serão listadas. |
|  `R6 - Busca de Disciplinas` |  Disciplinas poderão ser buscadas diretamente pelo seu código ou nome. Ao acessar a página da disciplina, será possível visualizar informações básicas sobre ela. |
|  `R7 - Export de Informações` |  Para cada disciplina será possível realizar a exportação de um relatório em PDF, trazendo detalhes mais ricos a respeito de sua ementa e conteúdos programáticos. |
|  `R8 - Log de Atividades` | Todas as alterações realizadas no sistema em produção ficarão registradas em uma tabela, guardando o ID do usuário, a data, o objeto modificado e o IP de acesso. |