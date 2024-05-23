# Curso Vue.js - Laravue

## Diretivas
- Diretiva é uma instrução ou conjunto de instruções para a execução de uma ação

- No contexto do Vue, diretivas são elementos que adicionamos as tags html para dar instruções a um bloco de código

- Toda diretiva no Vue é precedida por `v-`

```javascript

    <div v-if="true">
        {{ title }}
    </div>

    <div v-if="false">
        {{ title }}
    </div>
    
```

- Diretiva `v-show` serve para mostrar e ocultar elementos do html do DOM

- Diretiva `v-if` é semelhante a `v-show` a diferença entre elas é que a diretiva `v-if` remove o elemento do DOM ao invés de aplicar um estilo `display: none`, além disso, o Vue insere um comentário no DOM no lugar do elemento `<!--v-if-->`

- A diretiva `v-else` é um complemento da diretiva `v-if`, ou seja, ela funciona com a mesma lógica do `else` em qualquer linguagem

- Existe também a diretiva `v-else-if` que segue a mesma lógica de qualquer linguagem de programação

- Podemos usar a tag nativa `template` do html juntamente com a diretiva `v-if` quando não quisermos renderizar uma div pai
    - A tag `<template>`é utilizada para armazenar fragmentos de conteúdo HTML que podem ser clonados e inseridos no documento, mas que não são exibidos na página até serem explicitamente adicionados ao DOM (Document Object Model) por meio de scripts JavaScript. Essa tag é muito útil para criar componentes reutilizáveis ou para gerar conteúdo dinamicamente.

- A diretiva `v-for` serve para criar iterações com um elemento iterável e usa a sintaxe `alias in expression` para fornecer um pseudônimo para o elemento atual a ser iterado 

- A diretiva `v-bind` serve para preencher **qualquer atributo** das tags html e a sintaxe usada é a seguinte `v-bind:atributo='variavel'`
    - `v-bind` cria uma **interligação de mão única** (one-way binding), ou seja, em um único sentido (Data -> View), de forma que qualquer alteração nos dados do componente será refletida na visualização, mas não o contrário. 

- A diretiva `v-model` pode ser usada para criar **interligações de mão dupla** (two-way binding) entre os dados e elementos input, textarea e select de formulários