# Planejamento de Testes

### Definições:
- Tecnologias
  - Jest and Supertest
- Ponto de Partida
  - Testes Unitários (validar os inputs e o comportamento dos métodos com seus respectivos retornos e tratamentos de erros).
- Método
  - Execução manual em ambiente local.
  - Execução automatizada em gitflow, realizada via script a cada deploy.
- Justificativa
  - A quantidade estimada de testes é justificada pelo número de rotas expostas considerando, no mínimo, um teste para o bom comportamento e o mau comportamento desses componentes.

| Testes Unitários | Módulo de Disciplinas |
|---------|-----------------|
| *Quantidade Estimada* | 5 |
| *Prioridade* | Altíssima |

- **`should be able to create a imported component`**: Para que esse teste passe, sua aplicação deve criar os componentes através da importação do SIAC, utilizando a rota do crawler. Lembre-se que, de acordo à arquitetura do projeto, quando uma disciplina é criada uma cópia também é criada na tabela de draft.
- **`should be able to create a component`**: Para que esse teste passe, sua aplicação deve criar com sucesso e retornar um objeto do tipo disciplina ou código 201. Lembre-se que, de acordo à arquitetura do projeto, quando uma disciplina é criada uma cópia também é criada na tabela de draft.
- **`should not be able to create component with same code`**: Para que esse teste passe, sua aplicação deve retornar 400 ao tentar criar um novo objeto do tipo disciplina que contenha um código igual ao de outro objeto disciplina já existente.
- **`should not be able to create new Component without auth user`**: Para que esse teste passe, sua aplicação deve retornar 400 ao tentar criar um novo objeto do tipo disciplina com um usuário não autenticado.
- **`should not be able to create new component with empty body`**: Para que esse teste passe, sua aplicação deve retornar 400 ao receber uma requisição vazia.
- **`should be able to list the components`**: Para que esse teste passe, sua aplicação deve retornar um array de disciplinas.
- **`should be able to list the component by id`**: Para que esse teste passe, sua aplicação deve retornar um objeto do tipo disciplina referente a disciplina encontrada para o respectivo id.
- **`should be able to list the components filtered by name or code`**: Para que esse teste passe, sua aplicação deve retornar um array de disciplinas que deem match com um nome ou código.

| Testes Unitários | Módulo de Auth |
|---------|-----------------|
| *Quantidade Estimada* | 3 |
| *Prioridade* | Alta |

- **`should be able to login`**: Para que esse teste passe, sua aplicação deve receber os devidos parâmetros de login e validar a existência de um usuário, retornando então o token autenticado.
- **`should not be able to login user with incorrect email and/or password`**: Para que esse teste passe, sua aplicação deve receber um email ou senha inválidos e retornar o código 400.
- **`should not be able to login user without email`**: Para que esse teste passe, sua aplicação deve receber apenas uma senha e retornar o código 400.
- **`should not be able to login user without password`**: Para que esse teste passe, sua aplicação deve receber apenas um email e retornar o código 400.
- **`should not be able to login user with empty body`**: Para que esse teste passe, sua aplicação deve receber uma requisição vazia e retornar o código 400.
- **`should be able to reset user password`**: Para que esse teste passe, sua aplicação deve receber um email e validar a existência de um usuário, criando uma nova senha aleatória a ser enviada para o email do mesmo.
- **`should not be able to reset password user with incorrect email`**: Para que esse teste passe, sua aplicação deve receber um email e validar a inexistência de um usuário e retornar o código 400.
- **`should be able to create an invite`**: Para que esse teste passe, sua aplicação deve retornar um link válido (com validade de 24h) a ser utilizado para outros usuários se cadastrarem.

| Testes Unitários | Módulo de Usuários |
|---------|-----------------|
| *Quantidade Estimada* | 3 |
| *Prioridade* | Média |

- **`should be able to create a user`**: Para que esse teste passe, sua aplicação deve criar com sucesso e retornar um objeto do tipo usuário ou código 201. Lembre-se que o cadastro de um usuário está atrelado à lógica de Convite para cadastro.
- **`should be able to update a user`**: Para que esse teste passe, sua aplicação deve editar com sucesso as informações de um usuário e retornar o código 200.
- **`should be able to list a user by id`**: Para que esse teste passe, sua aplicação deve retornar um objeto do tipo usuário respectivo ao id passado.

| Testes de Integração | Módulo de Usuário + Disciplina |
|---------|-----------------|
| *Quantidade Estimada* | 5 |
| *Prioridade* | Altíssima |

| Testes de Integração | Módulo de Usuário + Auth |
|---------|-----------------|
| *Quantidade Estimada* | 3 |
| *Prioridade* | Alta |

| Testes Manuais Exploratórios | Todo o Sistema |
|---------|-----------------|
| *Quantidade Estimada* | 5 |
| *Prioridade* | Baixa |
