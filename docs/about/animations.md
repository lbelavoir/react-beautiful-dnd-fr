# Des animations soigneusement conçues

Lorsque les choses bougent beaucoup, il est facile pour l’utilisateur de se laisser distraire par les animations ou de se mettre en travers de l'une d'elle. Nous avons peaufiné les différentes animations pour assurer le bon équilibre entre guidage, performance et interactivité.

## Déposer

Nous avons conçu une animation de dépôt qui semble pondérée et physique. Il est basé sur un [`ressort`](https://developer.android.com/guide/topics/graphics/spring-animation) et utilise une animation CSS avec une durée dynamique pour obtenir l'effet.

![resultat-de-la-courbe](https://user-images.githubusercontent.com/2182637/48235467-1ce34200-e412-11e8-8c69-2060a0c2f61a.png)

> Courbe d'animation utilisée lors du déposer. La durée est dynamique en fonction de la distance à parcourir

Vous pouvez modifier l'animation déposer si vous le souhaitez. Nous avons créé un guide: [animation du déposer](/docs/guides/drop-animation.md)

## Déplacer hors des limites

Les éléments qui sont déplacés hors des limites d'un élément de glisser-déposer, le font avec une animation CSS plutôt que physiques. Cela permet d'optimiser les performances en permettant au GPU de gérer le mouvement. La courbe d'animation CSS a été conçue pour communiquer lors de la libération de l'élément.

Comment est-il composé:

1. Une période d'échauffement imitant un temps de réponse naturel
2. Une petite phase pour sortir rapidement de l'animation
3. Une longue queue pour que les gens puissent lire n'importe quel texte animé dans la seconde moitié de l'animation

![animation curve](https://raw.githubusercontent.com/alexreardon/files/master/resources/dnd-ease-in-out-small.png?raw=true)

> Animation curve used when moving out of the way

[← Back to documentation](/README.md#documentation-)
