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