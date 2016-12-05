---
layout: post
title:  "Impulsionando as tarefas do front-end"
date:   2016-12-05 12:30:00 -0300
categories: front-end
---

Olá!

Hoje eu estou lançando no meu Github um projeto chamado [Front-end startup](https://github.com/barbier/front-end-startup). A ideia é que ele possa ajudar a acelerar o desenvolvimento e economizar tempo na criação de tarefas básicas como compilar arquivos less e minificar javascripts.

## Dependências

Você precisa ter o [Node.js](https://nodejs.org/en/) e NPM instalados. Normalmente o NPM é instalado junto com o Node.

## Instalação e uso

Clone o projeto e execute `npm install` no seu terminal.

Para executar, digite `gulp` e o [Gulp](http://gulpjs.com/) irá executar a tarefa `default` (padrão).

## Lista de tarefas

- less: Compila todos os arquivos [less](http://lesscss.org/) presentes no diretório src em um único arquivo css otimizado com [csso](https://github.com/css/csso).
- js: Concatena e minifica todo os arquivos javascript nos diretórios src e vendor em um único arquivo. Preste atenção nas dependências no diretório vendor, é uma boa ideia colocar os arquivos manualmente numa ordem para evitar que o script final tenha problemas de execução.
- server: Executa um [servidor Browser Sync](https://www.browsersync.io/) para desenvolvimento mobile e desktop. Ele irá dar watch em alterações nos arquivos less, js e html e recarregar a página atual.

Espero que vocês gostem deste projeto e que seja útil para vocês. Há algumas issues que eu gostaria de discutir futuras abordagens para a manutenção do mesmo.
