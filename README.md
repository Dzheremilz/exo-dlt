# exo-dlt

- Comment est géré le cas ou le nombre de transactions dans le Block à valider est impair pour générer un `Merlke root` ?

![Foo](https://www.derpturkey.com/content/images/2020/07/merkle_construct_3.jpg)

On combine avec lui-meme le node qui se retrouve seul

- Dans le réseau bitcoin, Comment un nouveau noeud arrive t'il à retrouver ses pairs et ainsi rejoindre le réseau ?

En utilisant la plus longue chaine de proof-of-work qui fait référence

- Pouvez vous nommer au moins une personne qui a ou aurait pu influencer directement ou indirectement la création de Bitcoin par ses travaux (une personne qui n'a pas été nommée dans le cours)?

Wei Dai, concepteur de la b-money

- Avec vos propres recherches et grâce aux compétences acquises en cours pouvez vous expliquer comment une Blockchain crée un lien entre ses différents Blocks?

Quand un block est accepté, le suivant est crée utilisant le hash du block dernièrement accepté, c'est ainsi qu'ils sont chainés, le dernier block pointe vers le précédent

- Quelle structure de données informatique peut représenter le mieux cette chaine de Block: https://en.wikipedia.org/wiki/List_of_data_structures ?

Une liste chainée inversé, chaque élément pointant vers le précédent

- Si je souhaite modifier une transaction de 10 bitcoin que j'ai effectué il y a 6 mois en une transaction de 1 Bitcoin, que dois je modifier dans la Blockchain et que dois je mettre en oeuvre pour que cette modification persiste ?
Est ce possible selon vous ?

Il faudrait pouvoir modifier le block contenant la transaction ( refaire la proof-of-work) ainsi que tout les suivants, les données des transactions étant utilise pour crée le hash se transmetant d'un block a l'autre.
Meme en s'y prenant directement, tenter de crée une chaine alternative a très peu de chance de réussir