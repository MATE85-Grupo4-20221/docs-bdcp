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
  - A quantidade estimada de testes é justificada pelo número de rotas expostas considerando, no mínimo, um teste para o bom compartamento e o mau comportamento desses componentes. 

| Testes Unitários | Módulo de Disciplinas |
|---------|-----------------|
| *Quanidade Estimada* | 20 |
| *Prioridade* | Altíssima |

| Testes Unitários | Módulo de Auth |
|---------|-----------------|
| *Quanidade Estimada* | 5 |
| *Prioridade* | Alta |

| Testes Unitários | Módulo de Usuários |
|---------|-----------------|
| *Quanidade Estimada* | 10 |
| *Prioridade* | Média |

| Testes de Integração | Módulo de Usuário + Disciplina |
|---------|-----------------|
| *Quanidade Estimada* | 5 |
| *Prioridade* | Altíssima |

| Testes de Integração | Módulo de Usuário + Auth |
|---------|-----------------|
| *Quanidade Estimada* | 3 |
| *Prioridade* | Alta |

| Testes Manuais Exploratórios | Todo o Sistema |
|---------|-----------------|
| *Quanidade Estimada* | 5 |
| *Prioridade* | Baixa |
