---
layout: default
title: Sujet de stage
---
# Production d'un outil open source pour la compression de maillages volumiques 3D

**Encadrant.e.s et équipe :** Frédéric Payan (Mediacoding / SIS)

**Contact :**
fpayan@i3s.unice.fr

### Description

HexaShrink [1] est un outil permettant de décomposer efficacement des représentations numériques de sous-sols à différentes résolutions. Ces sous-sols sont modélisés à l'aide de maillages volumiques combinant géométrie 3D et propriétés physiques. Une animation est disponible à : http://laurent-duval.eu/opus-hexashrink-multiscale-mesh-representation-compression-wavelet-modelet.html

Il a été démontré que l'application d'une transformation en loi de puissance (autrement dit un compandeur [2]) sur ces modèles volumiques améliorait significativement des applications telles que la compression progressive ou encore la simulation numérique [3].

L'objectif de ce tutorat sera dans un premier temps d'implémenter une fonction python qui prend en entrée les données numériques et y applique un compandeur (ainsi que sa fonction inverse). Une validation sera effectuée sur le modèle 3D open data nommé LUNDIsim [4].

Dans un second temps, cette fonction sera interfacée avec un outil de compression de données 3D nommé SPIHT3D [5].

L'objectif du livrable final sera de produire un outil de démonstration open source qui sera rendu public.

[1] Peyrot, JL., Duval, L., Payan, F. et al. HexaShrink, an exact scalable framework for hexahedral meshes with attributes and discontinuities: multiresolution rendering and storage of geoscience models. Comput Geosci. https://doi.org/10.1007/s10596-019-9816-2
[2] https://en.wikipedia.org/wiki/Companding
[3] https://youtu.be/48F9-kSjczs
[4] https://zenodo.org/records/14641959
[5] https://github.com/echristophe/3d_spiht_rars

