# Qu'est- ce qu'un mesh 3d

> Avant de commencer à modéliser, nous devons comprendre comment fonctionne un mesh.

Un mesh est défini dans un espace tridimensionnel, sous forme de __points (vertices)__ ,__d'arêtes (edges)__ et de __faces__ :

![image](/ressources/mesh_3d/composants_mesh.png)

- Chaque __vertex__  est défini par trois valeurs, X, Y et Z, indiquant sa position dans le monde.

- __Un edge__ est une ligne formées en connectant 2 vertices.

## Les types de faces

Il existe trois types de faces/polygones : 

![image](/ressources/mesh_3d/ngon_definition.gif)

1. __Le triangle__ a trois cotés. C'est la face de base composant un mesh, il ne peut être que plat.

2. __Un quad__ a quatres côtés. Il est composé de deux triangles.

3. __Un Ngon__ a plus de quatres côtés. On peut aussi dire qu'il est composé de plus que deux triangles.



### Les autres propriétés des faces

Une face peut être de type "single-sided" ou "double-sided" :

Les faces "single-sided" sont invisibles de l'arrière. 
Les faces "double-sided" sont visibles de l'arrière.

Les polygones sont "infiniment plats" et semblent invisibles de côté en raison de leur absence d'épaisseur.

Chaque face de polygone a une "normale", déterminant comment la lumière réagis à sa surface ("shading").

Les objets complexes en 3D sont composés de nombreux polygones, avec plus de polygones nécessaires pour les objets ayant des surfaces courbes. 
Avec suffisamment de polygones, n'importe quelle forme solide en 3D peut être sculptée.

## Démo vidéo

[video youtube](https://www.youtube.com/embed/-bZ7gstIWyI" ':include :type=iframe width=100% height=400px')

