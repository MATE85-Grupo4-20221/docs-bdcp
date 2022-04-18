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
| *Quantidade Estimada* | 20 |
| *Prioridade* | Altíssima |

| Testes Unitários | Módulo de Auth |
|---------|-----------------|
| *Quantidade Estimada* | 5 |
| *Prioridade* | Alta |

| Testes Unitários | Módulo de Usuários |
|---------|-----------------|
| *Quantidade Estimada* | 10 |
| *Prioridade* | Média |

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
