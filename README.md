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
- [ ] Configurando Webpack
- [ ] Estrutura do ReactJS
- [ ] Servindo HTML estático
- [ ] Webpack Dev Server
- [ ] Utilizando source maps
- [ ] Ambiente dev e produção
- [ ] Importando arquivos CSS
- [ ] Utilizando SASS
</details>

<details>
<summary>2. Conceitos importantes</summary>

 - [ ] Primeiro componente React
 - [ ] Propriedades no React
 - [ ] Estado do componente
 - [ ] A imutabilidade no React
 - [ ] Fast Refresh no Webpack
</details>

<details>
<summary>3. Chamadas HTTP</summary>

 - [ ] Estilização da listagem
 - [ ] Utilizando o useEffect
 - [ ] Listando repositórios
</details>

<details>
<summary>4. Usando TypeScript</summary>

 - [ ] Fundamentos do TypeScript
 - [ ] TypeScript no ReactJS
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

    <tipo>[escopo]: <descrição>

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
