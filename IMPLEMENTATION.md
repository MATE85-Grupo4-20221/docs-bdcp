# Documentação de Implementação

- Implementação 

| Requisitos Mínimos (recomendado para desenvolvimento) | Descrição |
| --------- | --------- |
| `Sistema Operacional` | Linux Ubuntu v20.04 |
| `Memória RAM` | 8gb |
| `Browser WEB` | Google Chrome |

| Tecnologias | Descrição |
| --------- | --------- |
| `Engine` | NodeJs v16.13.2 |
| `Gerenciador de Pacotes` | NPM v8.1.2 |
| `Banco de Dados` | Postgresql |
| `Container` | Docker v20.01 |

| Acessos | Descrição |
| --------- | --------- |
| `Acesso Local Frontend` | localhost:3000 |
| `Acesso Local Backend` | localhost:3333, localhost:3333/api/docs |

- First Steps
1. Faça o clone dos repositórios backend e frontend respectivamente abaixo:

```sh
  $ git clone https://github.com/MATE85-Grupo4-20221/api-bdcp.git
  $ git clone https://github.com/MATE85-Grupo4-20221/app-bdcp.git
```

2. Executando a Aplicação Backend:
 ```sh
    # Abra o repositório em seu editor preferido
    $ cd /api-bdcp
 
    # Instale as dependências
    $ npm install
    
    # Faça uma cópia do arquivo **.env.example** e renomeie-o apenas para **.env**
    # É neste arquivo que estão definidas as variáveis de conexão com o banco. 
    
    # Execute o script de criação do banco de dados postgres.
    # Nesta etapa é imprescindível que tenha instalado o docker em sua máquina. Caso não tenha e opte por fazer a configuração manual do banco, não esqueça de checar as variáveis de configuração no arquivo **.env**
    $ npm run postgres:create
    
    # Finalmente, execute o comando para rodar a aplicação, que ficará disponível em localhost:3333.
    $ npm run dev
 ```

3. Executando a Aplicação Frontend:
