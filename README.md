# Sample Vue Atomic Frame Structure

├── assets
│   ├── styles
│       ├── [app.scss](#app.scss)
│       ├── style.scss
├── components
│   ├── atoms
│   ├── molecules
│   ├── organisms
│   ├── templates
├── composables
├── modules
├── pages
├── repositories
│   ├── client
│   ├── RepositoryFactory.ts
│   ├── someFactory.ts
├── router
├── store
├── App.vue
└── main.ts

#app.scss
Contains the common style sheet for the app.


[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin) to make the TypeScript language service aware of `.vue` types.

If the standalone TypeScript plugin doesn't feel fast enough to you, Volar has also implemented a [Take Over Mode](https://github.com/johnsoncodehk/volar/discussions/471#discussioncomment-1361669) that is more performant. You can enable it by the following steps:

1. Disable the built-in TypeScript Extension
    1) Run `Extensions: Show Built-in Extensions` from VSCode's command palette
    2) Find `TypeScript and JavaScript Language Features`, right click and select `Disable (Workspace)`
2. Reload the VSCode window by running `Developer: Reload Window` from the command palette.

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```
* [src/](.\vue_atomic_ojt\src)
  * [assets/](.\vue_atomic_ojt\src\assets)
    * [styles/](.\vue_atomic_ojt\src\assets\styles)
      * [foundation/](.\vue_atomic_ojt\src\assets\styles\foundation)
        * [settings/](.\vue_atomic_ojt\src\assets\styles\foundation\settings)
        * [_base.scss](.\vue_atomic_ojt\src\assets\styles\foundation\_base.scss)
        * [_reset.scss](.\vue_atomic_ojt\src\assets\styles\foundation\_reset.scss)
      * [app.scss](.\vue_atomic_ojt\src\assets\styles\app.scss)
      * [styles.scss](.\vue_atomic_ojt\src\assets\styles\styles.scss)
  * [components/](.\vue_atomic_ojt\src\components)
    * [atoms/](.\vue_atomic_ojt\src\components\atoms)
      * [VAlert/](.\vue_atomic_ojt\src\components\atoms\VAlert)
        * [VAlert.vue](.\vue_atomic_ojt\src\components\atoms\VAlert\VAlert.vue)
      * [VBtn/](.\vue_atomic_ojt\src\components\atoms\VBtn)
        * [VBtn.vue](.\vue_atomic_ojt\src\components\atoms\VBtn\VBtn.vue)
      * [VError/](.\vue_atomic_ojt\src\components\atoms\VError)
        * [VError.vue](.\vue_atomic_ojt\src\components\atoms\VError\VError.vue)
      * [VInputText/](.\vue_atomic_ojt\src\components\atoms\VInputText)
        * [VInputText.vue](.\vue_atomic_ojt\src\components\atoms\VInputText\VInputText.vue)
      * [.gitkeep](.\vue_atomic_ojt\src\components\atoms\.gitkeep)
    * [molecules/](.\vue_atomic_ojt\src\components\molecules)
      * [VFormControl/](.\vue_atomic_ojt\src\components\molecules\VFormControl)
        * [VFormControl.vue](.\vue_atomic_ojt\src\components\molecules\VFormControl\VFormControl.vue)
      * [.gitkeep](.\vue_atomic_ojt\src\components\molecules\.gitkeep)
    * [organisms/](.\vue_atomic_ojt\src\components\organisms)
      * [.gitkeep](.\vue_atomic_ojt\src\components\organisms\.gitkeep)
      * [NavBar.vue](.\vue_atomic_ojt\src\components\organisms\NavBar.vue)
    * [templates/](.\vue_atomic_ojt\src\components\templates)
      * [.gitkeep](.\vue_atomic_ojt\src\components\templates\.gitkeep)
      * [FormTemplate.vue](.\vue_atomic_ojt\src\components\templates\FormTemplate.vue)
  * [composables/](.\vue_atomic_ojt\src\composables)
    * [useLogin.ts](.\vue_atomic_ojt\src\composables\useLogin.ts)
  * [modules/](.\vue_atomic_ojt\src\modules)
    * [Login.ts](.\vue_atomic_ojt\src\modules\Login.ts)
  * [pages/](.\vue_atomic_ojt\src\pages)
    * [Login.vue](.\vue_atomic_ojt\src\pages\Login.vue)
    * [Welcome.vue](.\vue_atomic_ojt\src\pages\Welcome.vue)
  * [repositories/](.\vue_atomic_ojt\src\repositories)
    * [client/](.\vue_atomic_ojt\src\repositories\client)
      * [ApiAxiosClient.ts](.\vue_atomic_ojt\src\repositories\client\ApiAxiosClient.ts)
    * [loginRepository.ts](.\vue_atomic_ojt\src\repositories\loginRepository.ts)
    * [RepositoryFactory.ts](.\vue_atomic_ojt\src\repositories\RepositoryFactory.ts)
  * [router/](.\vue_atomic_ojt\src\router)
    * [index.ts](.\vue_atomic_ojt\src\router\index.ts)
  * [store/](.\vue_atomic_ojt\src\store)
    * [index.ts](.\vue_atomic_ojt\src\store\index.ts)
  * [App.vue](.\vue_atomic_ojt\src\App.vue)
  * [main.ts](.\vue_atomic_ojt\src\main.ts
