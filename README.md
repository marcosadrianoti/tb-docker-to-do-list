# Projeto Docker Todo List! :memo:
Projeto desenvolvido por mim durante o curso de Desenvolvimento Web na Trybe. Divulgado aqui como portfólio de aprendizado.

<details>
<summary><strong>Objetivos do projeto:</strong></summary>

  * Temos um aplicativo de `tarefas`! Esta aplicação precisa ser _conteinerizada_ com `Docker` para funcionar. Você deverá desenvolver os arquivos de configuração para cada frente específica: `Front-end`, `Back-end` e um aplicativo de `teste`.
  * Verificar se eu era capaz de:
    * Conteinerizar aplicações.
    * Criar uma conexão entre elas.
    * Orquestrar seu funcionamento.
</details>
<details>
<summary><strong> Requisitos do projeto:</strong></summary>

  * Criar um container em modo interativo, sem rodá-lo, nomeando-o como `01container` e utilizando a imagem `alpine` na versão `3.12`.
  * Iniciar o container `01container`.
  * Listar os containers filtrando pelo nome `01container`.
  * Executar o comando `cat /etc/os-release` no container `01container` sem se acoplar a ele.
  * Remover o container `01container`.
  * Fazer o download da imagem `nginx` com a versão `1.21.3-alpine` sem criar ou rodar um container.
  * Rodar um novo container com a imagem `nginx` com a versão `1.21.3-alpine` em segundo plano nomeando-o como `02images` e mapeando sua porta padrão de acesso para porta `3000` do sistema hospedeiro.
  * Parar o container `02images` que está em andamento.
  * Gerar uma build a partir do Dockerfile do `back-end` do `todo-app` nomeando a imagem para `todobackend`.
  * Gerar uma build a partir do Dockerfile do `front-end` do `todo-app` nomeando a imagem para `todofrontend`.
  * Gerar uma build a partir do Dockerfile dos `testes` do `todo-app` nomeando a imagem para `todotests`.
  * Bônus:
    * Subir uma orquestração em segundo plano com o docker-compose de forma que `backend`, `frontend` e `tests` consigam se comunicar.
</details>
  
## Rodando o projeto localmente

Para rodar o projeto em sua máquina, abra seu terminal, crie um diretório no local de sua preferência com o comando `mkdir` e acesse o diretório criado com o comando `cd`:

```bash
mkdir meu-diretorio &&
cd meu-diretorio
```

Clone o projeto com o comando `git clone`:

```bash
git clone git@github.com:marcosadrianoti/tb-docker-to-do-list.git
```

Acesse o diretório do projeto com o comando `cd`:

```bash
cd tb-docker-to-do-list
```

Instale as dependências executando:

```bash
npm install
```

Para executar os testes, É necessário ter o [Docker](https://www.docker.com/) instalado corretamente na sua máquina:

```bash
npm run test
```
