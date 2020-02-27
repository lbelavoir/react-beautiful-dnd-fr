# Installation

[![module formats: umd, cjs, et esm](https://img.shields.io/badge/module%20formats-umd%2c%20cjs%2c%20esm-green.svg?style=flat)](https://unpkg.com/react-beautiful-dnd/dist/)

## Général

1. Ajouter le paquet `react-beautiful-dnd`

```bash
# yarn
yarn add react-beautiful-dnd

# npm
npm install react-beautiful-dnd --save
```

2. Utiliser le paquet

```js
import { DragDropContext } from "react-beautiful-dnd";
```

3. Bénéfice 🕺

## Environnement `React`

Afin d'utiliser `react-beautiful-dnd` vous devrez installer un environnement `React`.

- [Ajouter react à un site web](https://reactjs.org/docs/add-react-to-a-website.html) - documentation officielle de `React`
- [Installer un environnement react avec `create-react-app`](https://egghead.io/lessons/react-set-up-a-react-environment-with-create-react-app) - suivant notre [leçon gratuite pour démarrer](https://egghead.io/courses/beautiful-and-accessible-drag-and-drop-with-react-beautiful-dnd)

## Paquet de distribution

Un ensemble [de définition du module universel](https://github.com/umdjs/umd) est publié sur `npm` dans le fichier `/dist` prêt pour l'utilisation. Nous publions les fichiers suivants:

- `dist/react-beautiful-dnd.js`
- `dist/react-beautiful-dnd.min.js` (module minifié)

Ces paquets listent `react` comme une ressource externe qui doit être fournies. Le but est de réduire la taille du paquet et d'éviter les utilisateurs de charger `react` plusieurs fois. Vous pouvez fournir `react` depuis votre système ou simplement en ayant `react` dans `window`.

Vous pouvez utiliser le UMD pour faire fonctionner `react-beautiful-dnd` directement dans le navigateur.

```html
<!-- dépendence pair -->
<script src="https://unpkg.com/react@16.3.1/umd/react.development.js"></script>
<!-- bibliothèque (changez x.x.x pour le numéro de version que vous désirez) -->
<script src="https://unpkg.com/react-beautiful-dnd@x.x.x/dist/react-beautiful-dnd.js"></script>
<!-- nécessaire pour monter votre application react -->
<script src="https://unpkg.com/react-dom@16.3.1/umd/react-dom.development.js"></script>

<script>
  const React = window.React;
  const ReactDOM = window.ReactDOM;
  const { DragDropContext, Draggable, Droppable } = window.ReactBeautifulDnd;

  function App() {
    // ...
  }

  // Vous pouvez utiliser JSX si votre environnement le permet
  ReactDOM.render(React.createElement(App), document.getElementById("app"));
</script>
```

Il existe aussi un [exemple codepen](https://codepen.io/alexreardon/project/editor/ZyNMPo) que vous pouvez utiliser pour essayer cette méthode d'installation.

## [`ClojureScript`](https://clojurescript.org/)

Vous pouvez utiliser `react-beautiful-dnd` depuis `ClojureScript` grâce à [CLJSJS](https://cljsjs.github.io/)!

[← Retour à la documentation](/README.md#documentation-)
