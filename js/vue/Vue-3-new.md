# Vue 3 changed

https://www.youtube.com/watch?v=WmFSGNqgOwc

https://www.youtube.com/watch?v=A5cVyjrKx_Q

https://v3.vuejs.org/guide/migration/introduction.html

https://www.youtube.com/watch?v=iuabg-OylbA

![image-20200923122013598](assets/VueJS-3-new/image-20200923122013598.png)

![image-20200923130712295](assets/VueJS-3-new/image-20200923130712295.png)

# Fragment

https://v3.vuejs.org/guide/migration/fragments.html

https://v3.vuejs.org/guide/component-attrs.html

In Vue 3, components now have official support for multi-root node components, i.e., fragments!

```html
<!-- Layout.vue
	In 2.x, multi-root components were not supported and would emit a warning when a user accidentally created one. As a result, many components are wrapped in a single <div> in order to fix this error.
-->
<template>
  <div>
    <header>...</header>
    <main>...</main>
    <footer>...</footer>
  </div>
</template>
```

```html
<!-- Layout.vue 
	In 3.x, components now can have multiple root nodes! However, this does require developers to explicitly define where attributes should be distributed.
-->
<template>
  <header>...</header>
  <main v-bind="$attrs">...</main>
  <footer>...</footer>
</template>
```

# Composition API

 [Vue-3-Composition-API.md](Vue-3-Composition-API.md) 

# Migrate guide

[Release v3.0.0 One Piece · vuejs/vue-next (github.com)](https://github.com/vuejs/vue-next/releases/tag/v3.0.0)

[Introduction | Vue.js](https://v3.vuejs.org/guide/migration/introduction.html#overview)

[Migrating from Vue 2 | Vue Router (vuejs.org)](https://next.router.vuejs.org/guide/migration/index.html#breaking-changes)

[Migrating to 4.0 from 3.x | Vuex (vuejs.org)](https://next.vuex.vuejs.org/guide/migrating-to-4-0-from-3-x.html)