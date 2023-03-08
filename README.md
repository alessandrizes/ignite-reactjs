# Trilha Ignite ReactJS 2021
Hi everyone! Este repositório foi criado para servir como acompanhamento aos estudos da trilha **Ignite ReactJS 2021** da RocketSeat :rocket:
A trilha foi desenvolvida separada por x capítulos

## Chapter I
Fundamentos iniciais da programação da web com ReactJS, bibliotecas de superte a criação de (SPA)single page applications, construindo uma aplicação `create-react-app` totalmente do zero.

<details>
<summary>1. Configurando ambiente</summary>

- [x] Introdução do módulo
- [x] Ambiente de Desenvolvimento [guia](https://efficient-sloth-d85.notion.site/Ambiente-de-desenvolvimento-Trilha-ReactJS-e7a377d183134647a177b6a34785f8c3)
- [x] Criando estrutura do projeto

    // inicia o repositório criando um arquivo package.json

    `yarn init -y` 

    // instala o react no projeto

    `yarn add react` 

    // instala o react-dom para habilitar a árvore de elementos do HTML no react

    `yarn add react-dom`
- [x] Configurando Babel

    // instala o babel como dependencia de desenvolvimento para compilar javaScript

    `yarn add @babel/core @babel/cli @babel/preset-env -D`

    // compila arquivo index.jsx e cria um novo arquivo bundle.js

    `yarn babel src/index.jsx --out-file dist/bundle.js`

    // instala o babel/preset-react para compreensão do código react no browser
    
    `yarn add @babel/preset-react -D`
- [x] Configurando Webpack

    // instala o webpack para auxiliar na conversão de arquivos de diferentes tipos para o browser
    
    `yarn add webpack webpack-cli -D`

    // instala o babel-loader para integrar o babel com o webpack e compreensão dos arquivos .js

    `yarn add babel-loader -D` 

    // executa o webpack

    `yarn webpack`
- [x] Estrutura do ReactJS
- [x] Servindo HTML estático
    // adiciona html-webpack-plugin para injetar arquivo js no HTML automaticamente

    `yarn add html-webpack-plugin -D`
- [x] Webpack Dev Server
    // adiciona webpack-dev-server para automatizar observador de alterações no código

    `yarn add webpack-dev-server -D`

    // executa o webserver localmente

    `yarn webpack serve`
- [x] Utilizando source maps
- [x] Ambiente dev e produção

    // adiciona cross-env para definir variáveis de ambiente em qualquer sistema operacional

    `yarn add cross-env -D`
- [x] Importando arquivos CSS

    // adiciona style-loader e css-loader para compreensão dos arquivos .css

    `yarn add style-loader css-loader -D`
- [x] Utilizando SASS

    // adiciona SASS como preprocessador no projeto

    `yarn add sass-loader -D`

    `yarn add node-sass -D`

    // remove dependência do projeto

    `yarn remove sass`
</details>

<details>
<summary>2. Conceitos importantes</summary>

 - [x] Primeiro componente React
 - [x] Propriedades no React
 - [x] Estado do componente
 - [x] A imutabilidade no React
 - [x] Fast Refresh no Webpack

    // adiciona react-refresh para alterar e salvar o código mantendo estado dos componentes no browser

    `yarn add -D @pmmmwh/react-refresh-webpack-plugin react-refresh`
</details>

<details>
<summary>3. Chamadas HTTP</summary>

 - [x] Estilização da listagem
 - [x] Utilizando o useEffect
 - [x] Listando repositórios
</details>

<details>
<summary>4. Usando TypeScript</summary>

 - [x] Fundamentos do TypeScript

    // um superset para javaScript, exemplo:

    ```
    type User = {
        name: string
        email: string
        address: {
            city: string
            state?: string
        }
    }

    function showWelcomeMessage(user: User) {
        return `Welcome ${user.name}, your e-mail is ${user.email}. Your city is ${user.address.city} and your state is ${user.address.state}`
    }

    showWelcomeMessage({
        name:'John Doe',
        email: 'john@doe.com',
        address: {
            city: 'New York',
            state: 'NY'
        }
    })
    ```
    
 - [x] TypeScript no ReactJS

    // adiciona o typescript como uma dependência de desenvolvimento

    `yarn add typescript -D`

    // inicia o typescript na aplicação

    `yarn tsc --init`

    // adiciona @babel/preset-typescript para compreensão do typescript

    `yarn add @babel/preset-typescript -D `

    // adiciona @types/react e @types/react-dom para compreensão do typescript

    `yarn add @types/react-dom -D`

    `yarn add @types/react -D`

 - [ ] Componentes com TypeScript
</details>

<details>
<summary>5. Finalizando aplicação</summary>

 - [ ] Utilizando React DevTools
 - [ ] Finalização do módulo


</details></br>

# Padrão para os commits
 Documentação oficial: [Conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)

A mensagem do commit deve ser estruturada da seguinte forma:

    tipo(escopo): descrição

## O **tipo** deve seguir os seguintes mencionado abaixo:
- **fix:** um commit do tipo `fix` soluciona um problema na sua base de código, isso se correlaciona com PATCH do versionamento semântico.
- **feat:** um commit do tipo `feat` inclui um novo recurso na sua base de código, isso se correlaciona com MINOR do versionamento semântico.
- **chore:** um commit do tipo `chore` inclui uma manutenção regular do código, uma alteração de código que o usuário externo não verá, por exemplo: alteração para arquivo .gitignore, você também pode usar emojis para representar os tipos de confirmação.
- **docs:** um commit do tipo `docs` inclui tudo relacionado a documentação.
- **style:** um commit do tipo `style` inclui um recurso e atualizações relacionadas ao estilo.
- **refactor:** um commit do tipo `refactor` inclui uma refatoração de uma seção específica da base de código, um código que não corrige bug nem adiciona um recurso, por exemplo: você pode usar isso quando houver mudanças semânticas, como renomear um nome de variável ou função.
- **test:**  um commit do tipo `test` inclui tudo relacionado a testes, adicionando um novo teste ou fazendo alterações em um teste existente.
- **build:** um commit do tipo `build` inclui construção ou alterações relacionadas por exemplo: npm relacionado, adicionando dependências externas.
- **ci:** um commit do tipo `ci` inclui atualização do fluxo de trabalho.
- **perf:** um commit do tipo `perf` inclui um código que melhora o desempenho.
- **BREAKING CHANGE:** um commit que contém no rodapé opcional o texto `BREAKING CHANGE:`, ou contém o símbolo `!` depois do tipo/escopo, introduz uma modificação que quebra a compatibilidade da API (isso se correlaciona com MAJOR do versionamento semântico). Uma BREAKING CHANGE pode fazer parte de commits de qualquer tipo.
- **revert:** um commit do tipo `revert` é usado para reverter código.

## O **escopo** deve seguir os detalhes abaixo:
- É opcional.
- Caso inclua, deve ser um substantivo que representa a seção da seção da base de código, por exemplo: api, init, runner, watcher, config, web-server, proxy e etc.

## A **descrição** deve seguir os detalhes abaixo:
- Deve ser usado verbor no imperativo e no tempo presente, por exemplo: use "add" em vez de "added" ou "adds".
- Não use ponto (.) no final da sentença.
- Deve incluir a primeira letra sempre minúscula.
