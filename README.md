# Sample Vue Atomic Frame Structure

* src
  * assets
    * styles
      * [app.scss](#common-style)
      * [styles.scss](#scss-variable)
  * components
    * [atoms](#atoms)
    * [molecules](#molecules)
    * [organisms](#organisms)
    * [templates](#templates)
  * [composables](#composables)
  * [modules](#modules)
  * [pages](#pages)
  * repositories
    * [client](#client)
    * [RepositoryFactory.ts](#repository)
  * [router](#router)
  * [store](#store)
  * App.vue
  * main.ts

## Common Style
Contains the common style sheet for the app.

## Scss Variable
Contains the scss variable to use in all components.

## Atoms
Contains the app's atom components like buttons, links, input elements.

## Molecules
Contains the app's molecular level components like form control block.

## Organisms
Contains the app's organisms components like Navbar.

## Templates
Contains the app's templates level components like form template.

## Composables
Contain files that serves as a seperate data object for form and fetched api data. Set data which is fetched from api to this
composables files and get data from all other components.

## Modules
Contain files that export type as class constructor for each app's data.

## Pages
Contains app's pages.

## Client
Contains app's api fetching axios client initialization and configuration files.

## Repository
Repositories are api data fetching service for each app's data. Every different data must have its own repository and each repository shoud be extracted from RepositoryFactory.

## Router
Contains app's routing services.

## Store
Contains app's global store file.
