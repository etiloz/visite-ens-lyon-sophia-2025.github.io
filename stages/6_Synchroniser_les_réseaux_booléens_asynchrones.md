---
layout: default
title: Sujet de stage
---
# Synchroniser les réseaux booléens asynchrones

**Encadrant.e.s et équipe :** Adrien Richard et Florian Bridoux

**Contact :**
Adrien Richard, richard@unice.fr (https://webusers.i3s.unice.fr/~richard/)

### Description

Les réseaux d'automates modélisent des ensembles d’entités simples évoluant dans un temps discret et sur des domaines finis, selon des règles d’évolution locales. Ils trouvent de nombreuses applications — en biologie, sociologie ou informatique — car, malgré leur simplicité, ils engendrent une grande diversité de comportements dynamiques, faisant d’eux un cadre unificateur pour l’étude des systèmes complexes. Leur théorie relie des domaines variés — théorie des graphes, de la complexité, combinatoire, entre autres — et pose des questions fondamentales sur les relations entre structure, règles locales et comportements émergents.

On considère dans ce stage les réseaux booléens à n entités. Un tel réseau est décrit par une fonction f de l'ensemble des vecteurs binaires x=(x_1,...,x_n) à n composantes dans lui-même. Notons que chaque composante de f est une fonction booléenne à n composantes, notée f_i : c'est la fonction locale de la composante (ou entité) i. Ainsi, f(x)=(f_1(x),...,f_n(x)). 

On étudie souvent la dynamique synchrone de f, décrite par les itérations de f. Autrement dit, à chaque étape de temps, toutes les fonctions locales sont appliquées simultanément. Mais dans bien des applications, il est plus réaliste d'appliquer, à chaque étape de temps, une et une seule fonction locale : on parle de dynamique asynchrone. Plus précisément, appliquer la fonction locale f_i en x, c'est passer au vecteur (x_1,...,f_i(x),...,x_n), que l'on note f^i(x). Ainsi, f^i est un réseau booléen à n composantes. La collection des f^i forme un automate fini déterministe (AFD), appelé dynamique asynchrone de f :

- l'alphabet est {1,...,n},
- l'ensemble des états est l'ensemble des vecteurs binaires à n composantes, 
- la transition étiquetée par i partant de x mène à f^i(x).

Étant donné un mot sur l'alphabet {1,...,n}, on note f^w(x) l'état que l'on atteint depuis x en lisant le mot  w dans l'automate fini déterministe : si w=i_1,i_2,...,i_k alors f^w(x)=(f^{i_k} o ... o f^{i_2} o f^{i_1})(x). Ainsi, f^w est encore un réseau booléen à n composantes. On dit que w synchronise f si f^w est une fonction constante : quel que soit l'état initiale, la lecture de w mène toujours au même état. 

La synchronisation est un problème profond et très étudié. La conjecture la plus célèbre du domaine est la conjecture de Černý (1964) : si un AFD à q états a un mot synchronisant, alors il en a un de longueur au plus (q-1)^2. Le stage consiste à étudier cette conjecture dans le cas particulier des réseaux booléens : si f a un mot synchronisant, alors il en a un de longueur au plus (2^n-1)^2.

Ce cas particulier est intéressant à plusieurs points de vue. Les réseaux booléens ont de nombreuses applications, et leur synchronisation pourrait être une propriété cruciale dans certains cas. Ils sont par ailleurs très structurés : la dynamique asynchrone est essentiellement une orientation de l'hypercube, structure qui se prête particulièrement bien aux raisonnements par induction. De plus, la conjecture a été démontrée pour certaines familles d'AFDs, mais les réseaux booléens diffèrent complètement de ces familles ; leur étude pourrait donc ajouter une (très) nouvelle pierre à l'édifice. Enfin, quelques résultats partiels sont encourageants [1] et pourront servir de point de départ. 

[1] Synchronizing Boolean networks asynchronously,
    J. Aracena, A. Richard, L. Salinas.
    Journal of Computer and System Sciences, 136:249-279, 2023. 
    https://arxiv.org/abs/2203.05298


