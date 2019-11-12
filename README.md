<p align="center">
  <img src="https://user-images.githubusercontent.com/2182637/53611918-54c1ff80-3c24-11e9-9917-66ac3cef513d.png" alt="react beautiful dnd logo" />
</p>
<h1 align="center">react-beautiful-dnd <small><sup>(rbd)</sup></small></h1>

<div align="center">

**Élégant** et **accessible** glisser-déposer de listes en [`React`](https://facebook.github.io/react/)

[![Branche CircleCI](https://img.shields.io/circleci/project/github/atlassian/react-beautiful-dnd/master.svg)](https://circleci.com/gh/atlassian/react-beautiful-dnd/tree/master)
[![npm](https://img.shields.io/npm/v/react-beautiful-dnd.svg)](https://www.npmjs.com/package/react-beautiful-dnd)

![quote application example](https://user-images.githubusercontent.com/2182637/53614150-efbed780-3c2c-11e9-9204-a5d2e746faca.gif)

[Essayer cet exemple si vous le souhaitez!](https://react-beautiful-dnd.netlify.com/iframe.html?selectedKind=board&selectedStory=simple)

</div>

## Caractéristiques principales

- [Mouvement naturel](/docs/about/animations.md) et élégant des objets 💐
- [Accessible](/docs/about/accessibility.md): clavier efficace et prise en charge de lecteur d'écran ♿️
- [Extrêmement performant](/docs/support/media.md) 🚀
- Api puissante et épuré avec laquelle il est simple de démarrer
- Réagit extrêmement bien avec les intéractions des navigateurs standards
- [Style flexible](/docs/guides/preset-styles.md)
- Pas de création d'enrobage de nœud de dom additionnel - adapté à flexbox et à la gestion de focus !

## Bien démarrer 👩‍🏫

Nous avons créé [un cours gratuit sur `egghead.io` 🥚](https://egghead.io/courses/beautiful-and-accessible-drag-and-drop-with-react-beautiful-dnd?af=2jc3e4) afin de vous aider à démarrer avec `react-beautiful-dnd` aussi vite que possible.

[![logo-cours](https://user-images.githubusercontent.com/2182637/43372837-8c72d3f8-93e8-11e8-9d92-a82adde7718f.png)](https://egghead.io/courses/beautiful-and-accessible-drag-and-drop-with-react-beautiful-dnd?af=2jc3e4)

## Liste des fonctionnalités actuellement prises en charge ✅

- Listes verticales ↕
- Listes horizontales ↔
- Mouvements entre listes (▤ ↔ ▤)
- [Prise en charge de liste virtuelle 👾](/docs/patterns/virtual-lists.md) - déverrouille 10,000 objets @ 60fps
- [Fusion d'objets](/docs/guides/combining.md)
- Prise en charge de souris 🐭, clavier 🎹♿️ et d'écran tactile 👉📱 (mobile, tablette et autres)
- [Prise en charge du multi-glisser](/docs/patterns/multi-drag.md)
- Incroyable prise en charge de lecteur d'écran ♿️ - nous fournissons une expérience incroyable et hors des sentiers battus pour les lecteurs d'écrans en anglais 📦. Nous donnons également le complet contrôle de la personnalisation et de la prise en charge de l'internationalisation pour ceux qui le désirent 💖
- [Glisser conditionnel](/docs/api/draggable.md#optional-props) et [conditionnel déposer](/docs/api/droppable.md#conditionally-dropping)
- Listes multiples et indépendentes sur la même page
- Taille d'objet variable - les objets déplaçables peuvent avoir différentes hauteurs (pour les listes verticales) ou largeurs (pour les listes horizontales)
- [Ajout et suppression d'objets pendant le déplacement](/docs/guides/changes-while-dragging.md)
- Compatible avec le sémantique `<table>` réorganisation - [modèle de table](/docs/patterns/tables.md)
- [Défilement automatique](/docs/guides/auto-scrolling.md) - défilement automatique des conteneurs et de la fenêtre si nécessaire pendant un déplacement (même avec le clavier 🔥)
- Gestions personnalisées du déplacement - vous pouvez glisser un object entier en utilisant simplement une partie de celui-ci
- Possibilité de bouger l'object déplaçable dans un autre élément pendant le déplacement (clone, portail) - [Attribuer un nouveau parent à un `<Draggable />`](/docs/guides/reparenting.md)
- [Créer des expériences de glisser-déposer préparée à l'avance 🎮](/docs/sensors/sensor-api.md)
- Peut être étendu pour prendre en charge [tous les types de senseur que vous aimez 🕹](/docs/sensors/sensor-api.md)
- 🌲 Prise de charge d'arborescence à travers le paquet [`@atlaskit/tree`](https://atlaskit.atlassian.com/packages/core/tree)
- Une liste `<Droppable />` peut être un conteneur de défilement (sans un parent défilable) ou être l'enfant d'un conteneur de défilement (qui lui aussi n'a pas de parent défilable)
- Listes imbriquées indépendantes - une liste peut être l'enfant d'une autre liste, mais vous ne pouvez pas déplacer des objets depuis une liste parent vers une liste enfant
- Compatible avec un rendu côté serveur (SSR) - voir [resetServerContext()](/docs/api/reset-server-context.md)
- Fonctionne bien avec [les éléments interactifs imbriqués](/docs/api/draggable.md#interactive-child-elements-within-a-draggable-) par défaut

## Motivation 🤔

`react-beautiful-dnd` existe pour créer un beau glisser-déposer pour des listes que tout le monde peut utiliser - même ceux qui ne peuvent pas voir. Pour avoir une bonne vue d'ensemble de l'historique et des motivations de ce projet, vous pouvez jeter un oeil à ces ressources externes:

- 📖 [Repenser le glisser-déposer](https://medium.com/@alexandereardon/rethinking-drag-and-drop-d9f5770b4e6b)
- 🎧 [React podcast: rapide, accessible et élégant glisser-déposer](https://reactpodcast.simplecast.fm/17)

## Pas pour tous ✌️

Il existe de nombreuses bibliothèques qui permettent des interactions de glisser-déposer avec React. La plus connues d'entre elles est la fabuleuse [`react-dnd`](https://github.com/react-dnd/react-dnd). Elle fait un travail incroyable en fournissant un grand ensemble de primitives glisser-déposer qui fonctionnent [particulièrement bien](https://www.quirksmode.org/blog/archives/2009/09/the_html5_drag.html) avec la fonctionnalité de glisser-déposer extrêmement générique html5. `react-beautiful-dnd` est une abstraction de niveau supérieur spécialement conçue pour les listes (verticale, horizontale, mouvement entre les listes, listes imbriquées, etc.). Dans ce sous-ensemble de fonctionnalités `react-beautiful-dnd` offre une expérience de glisser-déposer puissante, naturelle et esthétique. Cependant, il ne fournit pas l'étendue des fonctionnalités offertes par `react-dnd`. Donc `react-beautiful-dnd` peut ne pas vous convenir selon votre case d'utilisation.

## Documentation 📖

### À propos 👋

- [Installation](/docs/about/installation.md)
- [Exemples et échantillons](/docs/about/examples.md)
- [Bien démarrer](https://egghead.io/courses/beautiful-and-accessible-drag-and-drop-with-react-beautiful-dnd?af=2jc3e4)
- [Principes du design](/docs/about/design-principles.md)
- [Animations](/docs/about/animations.md)
- [Accessibilité](/docs/about/accessibility.md)
- [Prise en charge des navigateurs](/docs/about/browser-support.md)

### Capteurs 🔉

> Les manières dont une personne peut commencer et contrôler un déplacement

- [Glisser avec la souris 🐭](/docs/sensors/mouse.md)
- [Glisser avec un écran tactile 👉📱](/docs/sensors/touch.md)
- [Glisser avec un clavier 🎹♿️](/docs/sensors/keyboard.md)
- [Créer votre propre capteur](/docs/sensors/sensor-api.md) (accepte tous types de senseurs ainsi que les expériences scénarisés)

### API 🏋️‍

![diagramme](https://user-images.githubusercontent.com/2182637/53607406-c8f3a780-3c12-11e9-979c-7f3b5bd1bfbd.gif)

- [`<DragDropContext />`](/docs/api/drag-drop-context.md) - _Englobe la partie de votre application où vous souhaitez activer le glisser-déposer_
- [`<Droppable />`](/docs/api/droppable.md) - _Une zone où l'on peut déposer des objets. Contient des objets `<Draggable />`_
- [`<Draggable />`](/docs/api/draggable.md) - _Objet qui peut être déplacé_
- [`resetServerContext()`](/docs/api/reset-server-context.md) - _Utilitaire pour le rendu côté serveur (SSR)_

### Guides 🗺

- [`<DragDropContext />` réponses](/docs/guides/responders.md) - _`onDragStart`, `onDragUpdate`, `onDragEnd` et `onBeforeDragStart`_
- [Combiner des `<Draggable />`](/docs/guides/combining.md)
- [Problêmes habituels lors de l'installation](/docs/guides/common-setup-issues.md)
- [Utiliser `innerRef`](/docs/guides/using-inner-ref.md)
- [Détection des problèmes d'installation et récupération des erreurs](/docs/guides/setup-problem-detection-and-error-recovery.md)
- [Règles pour `draggableId` et `droppableId`s](/docs/guides/identifiers.md)
- [Rétention de la focalisation du navigateur](/docs/guides/browser-focus.md)
- [Personnaliser ou ignorer l'animation de déposer](/docs/guides/drop-animation.md)
- [Défilement automatique](/docs/guides/auto-scrolling.md)
- [Controller le lecteur d'écran](/docs/guides/screen-reader.md)
- [Utiliser le `doctype` html5](/docs/guides/doctype.md)
- [`TypeScript` et `flow`](/docs/guides/types.md)
- [Déplacer des `<svg>`](/docs/guides/dragging-svgs.md)
- [Éviter que l'image clignote](/docs/guides/avoiding-image-flickering.md)
- [Styles prédéfinis non visibles](/docs/guides/preset-styles.md)
- [Comment nous détectons les conteneurs de défilement](/docs/guides/how-we-detect-scroll-containers.md)
- [Comment utilisons-nous les évenements du _dom_](/docs/guides/how-we-use-dom-events.md) - _Utile si vous avez besoin de construire par dessus `react-beautiful-dnd`_
- [Ajouter des `<Draggable />`s pendant un glisser (comportement de 11.x)](/docs/guides/changes-while-dragging.md) - _⚠️ Avancé_
- [Configuration de la politique de sécurité du contenu](/docs/guides/content-security-policy.md)

### Modèle 👷‍

- [Listes virtuelles 👾](/docs/patterns/virtual-lists.md)
- [Multi-glissage](/docs/patterns/multi-drag.md)
- [Tables](/docs/patterns/tables.md)
- [Attribuer un nouveau parent à un `<Draggable />`](/docs/guides/reparenting.md) - _Utiliser notre API de clonage ou votre propre portail_

### Soutien 👩‍⚕️

- [Santé du code](/docs/support/engineering-health.md)
- [Communauté et suppléments](/docs/support/community-and-addons.md)
- [Notes de parution et journal des modifications](https://github.com/atlassian/react-beautiful-dnd/releases)
- [Mettre à jour](/docs/support/upgrading.md)
- [Feuille de route](https://github.com/atlassian/react-beautiful-dnd/issues)
- [Media](/docs/support/media.md)

## Lire ceci dans un autre langage 🌎

- [![kr](https://raw.githubusercontent.com/gosquared/flags/master/flags/flags/shiny/24/South-Korea.png) **한글/Coréen**](https://github.com/LeeHyungGeun/react-beautiful-dnd-kr)
- [![ru](https://raw.githubusercontent.com/gosquared/flags/master/flags/flags/shiny/24/Russia.png) **На русском/Russe**](https://github.com/vtereshyn/react-beautiful-dnd-ru)
- [![pt](https://raw.githubusercontent.com/gosquared/flags/master/flags/flags/shiny/24/Brazil.png) **Português/Portugais**](https://github.com/dudestein/react-beautiful-dnd-pt)

## Author ✍️

Alex Reardon [@alexandereardon](https://twitter.com/alexandereardon)

## Collaborators 🤝

- Bogdan Chadkin [@IAmTrySound](https://twitter.com/IAmTrySound)
- Luke Batchelor [@alukebatchelor](https://twitter.com/alukebatchelor)
- Jared Crowe [@jaredjcrowe](https://twitter.com/jaredjcrowe)
- Many other [@Atlassian](https://twitter.com/Atlassian)'s!
