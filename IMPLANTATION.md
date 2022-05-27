# Documentação de Implantação

- Implantação 

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
| `Acesso Local Backend` | localhost:3333 |
| `Documentação Backend` | localhost:3333/api/docs |

---

### Requisitos Obrigatórios
1. Para executar este projeto localmente, você precisa primeiramente ter o [NodeJs](https://nodejs.org/en/) v16 instalado na sua máquina. Naturalmente, o NPM será instalado junto.
2. Você também precisará ter instalado em sua máquina o [Docker](https://www.docker.com/).
3. Caso ainda não tenha esses recursos em sua máquina ou tem dúvidas de que foi instalado corretamente, busque pela documentação oficial e depois volte para este material de implementação.

### Get Started
1. Faça o clone dos repositórios backend e frontend respectivamente abaixo:

```sh
  $ git clone https://github.com/MATE85-Grupo4-20221/api-bdcp.git
  $ git clone https://github.com/MATE85-Grupo4-20221/app-bdcp.git
```

2. Executando a Aplicação Backend:
 ```sh
    # Abra o repositório em seu editor preferido
    $ cd /api-bdcp
    
    # Mude para a branch de desenvolvimento
    $ git checkout dev
    
    # Faça uma cópia do arquivo .env.example e renomeie-o apenas para .env
    # É neste arquivo que estão definidas as variáveis de conexão com o banco. 
    $ cp .env.example .env
 
    # Instale as dependências
    $ npm install
    
    # Execute o comando abaixo apenas para garantir que está tudo certo com o eslint.
    $ npm run lint:fix
    
    # Execute o script de criação do banco de dados postgres.
    # Nesta etapa é imprescindível que tenha instalado o docker em sua máquina. 
    # Caso não tenha e opte por fazer a configuração manual do banco, não esqueça de checar as variáveis de configuração no arquivo .env
    $ npm run postgres:create
    
    # Finalmente, execute o comando para rodar a aplicação, que ficará disponível em localhost:3333
    $ npm run dev
 ```
  - Se tudo der certo, esta deve ser a visão do seu cmd.
  - ![cmd-api](https://user-images.githubusercontent.com/62779767/170699050-988336f6-f206-4a37-b74a-e9fceb02a998.png)

3. Executando a Aplicação Frontend:
 ```sh
    # Abra o repositório em seu editor preferido
    $ cd /app-bdcp
    
    # Mude para a branch de desenvolvimento
    $ git checkout develop
    
    # Faça uma cópia do arquivo .env.example e renomeie-o apenas para .env
    # É neste arquivo que estão definidas as variáveis de conexão com a API.
    $ cp .env.example .env
 
    # Instale as dependências
    $ npm install
    
    # Execute o comando abaixo apenas para garantir que está tudo certo com o eslint.
    $ npm run lint:fix
    
    # Finalmente, execute o comando para rodar a aplicação, que ficará disponível em localhost:3000
    $ npm run start
 ```
   - Se tudo der certo, esta deve ser a visão do seu cmd.
   - ![cmd-app](https://user-images.githubusercontent.com/62779767/170700192-326fb6e3-4851-4f27-8da4-462560cf333e.png)


 
 ### Next Steps
  1. Para ter acesso à todo o conteúdo da aplicação você deve criar um usuário (se cadastrar no sistema). Utilize de softwares como, por exemplo, [Insomnia](https://insomnia.rest/download) ou [Postman](https://www.postman.com/), acessando diretamente o endpoint de geração de link de cadastro.
  2. Abra o Insomnia e envie uma requisição do tipo get para http://localhost:3333/api/invite/generate e depois copie o token gerado.
    2.1. ![insomnia-invite-user](https://user-images.githubusercontent.com/62779767/170702107-d0cb39bf-0c26-4aa6-9af3-5143e518e550.png)
  3. Abra o navegador e utilize http://localhost:3000/api/invite/validate/token onde, no lugar de 'token' você deverá colar aquele hash gerado no Insomnia.
  4. Apartir disso você já consegue logar no sistema e utilizar de todas as funcionalidades.
  5. Acesse o endpoint http://localhost:3333/api/docs para saber como usar todos os endpoints da API e como integrar ao frontend.

### Observações
 - Todo o processo de instalação dos softwares, clonagem de repositório e instalação de dependências não deve ultrapassar um tempo médio de 10 minutos. Caso esse tempo seja ultrapassado, algo deu errado e, neste caso, você deve voltar o passo e tentar novamente.
 - Em caso de dúvida, consulte um dos desenvolvedores através do email do projeto 'bdcpicufba@gmail.com'.

---

