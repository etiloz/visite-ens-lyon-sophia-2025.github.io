---
layout: default
title: Sujet de stage
---
# Graphe d'interaction, propriétés dynamiques, et complexité des réseaux booléens

**Encadrant.e.s et équipe :** Adrien Richard et Florian Bridoux

**Contact :**
Adrien Richard, richard@unice.fr (https://webusers.i3s.unice.fr/~richard/)

### Description

Les réseaux d'automates modélisent des ensembles d’entités simples évoluant dans un temps discret et sur des domaines finis, selon des règles d’évolution locales. Ils trouvent de nombreuses applications — en biologie, sociologie ou informatique — car, malgré leur simplicité, ils engendrent une grande diversité de comportements dynamiques, faisant d’eux un cadre unificateur pour l’étude des systèmes complexes. Leur théorie relie des domaines variés — théorie des graphes, de la complexité, combinatoire, entre autres — et pose des questions fondamentales sur les relations entre structure, règles locales et comportements émergents.

On considère dans ce stage les réseaux booléens à n entités, dont la dynamique est décrite par les itérations d'une fonction f de l'ensemble des vecteurs binaires à n composantes dans lui-même ; elle peut être représentée par un graphe, appelé graphe synchrone, où chaque sommet (vecteur à n composantes) a un unique successeur (son image par f). Notons que chaque composante de f est une fonction booléenne à n composantes, qui peut être codée par une formule booléenne. 

Un théorème profond et récent est le suivant [1]. Soit P une propriété dynamique sur les graphes synchrones exprimable en logique du premier ordre. Une telle propriété est triviale si elle a un nombre fini de modèles ou de contre-modèles. Le théorème est : soit P non-trivial ; décider si le graphe synchrone d'un réseau booléen f (décrit composante à composante par des formules booléennes) satisfait P est NP-difficile ou coNP-difficile. Ainsi, toute propriété non-triviale est (très) difficile à tester, ce qui montre bien qu'il est difficile de comprendre les comportements globaux (P) à partir des règles locales (les fonctions booléennes). À ce titre, les réseaux booléens sont donc bien complexes. 

Tester si la dynamique d'un réseau booléen satisfait une certaine propriété P est naturel. Cependant, en pratique, dans bien des contextes, on ne possède qu'une information très partielle sur le réseau f. Par exemple, il est classique que la seule information disponible soit le graphe d'interaction de f : les sommets de G sont les n composantes, et il y a un arc de la composante j sur la composante i si la ième composante de f dépend de la composante j. Ainsi, G décrit les influences entres les n composantes du système. L'information portée par G est faible car l'ensemble des réseaux booléens dont le graphe d'interaction signé est G - noté F(G) - est en moyenne doublement exponentiel en n. Donc, si on ne connait que G, une question naturelle est de décider s'il EXISTE un réseau dans F(G) dont la dynamique satisfait la propriété P ; on dit alors (abusivement) que G satisfait P.

Dans l'esprit du théorème mentionné ci-dessus, le sujet du stage consiste à étudier la complexité de décider si un graphe G satisfait une propriété P exprimable en logique du premier ordre. En remplaçant f par G le théorème est faux : il est facile de trouver des propriétés P non-triviales telles qu'il est polynomial de décider si G satisfait P. Mais de façon très déroutante (et contrairement au cas ``signé'' [2]), on ne connait AUCUNE propriété P telle qu'il est NP-difficile de décider si G satisfait P ! Le but du stage est d'en trouver une ! Dans l'optique optimiste qu'une telle propriété serait trouvée rapidement, il s'agirait ensuite de trouver des familles de telles propriétés, les plus naturelles possibles. On pourrait aussi envisager de chercher des propriétés qui vont au-delà des classes NP et coNP.  

[1] Rice-like complexity lower bounds for Boolean and uniform automata networks,
    Goubault-Larrecq, Perrot, 
    preprint, 2025.
    https://arxiv.org/abs/2409.08762

[2] Complexity of fixed point counting problems in Boolean networks,
    Bridoux, Durbec, Perrot, Richard,
    Journal of Computer and System Sciences, 226:138-164, 2022.
    https://arxiv.org/abs/2012.02513
    


