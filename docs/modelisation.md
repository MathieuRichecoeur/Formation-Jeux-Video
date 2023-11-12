# Modelisation sur Maya

Nous modélisons sur Maya, mais la majorité des concepts abordés sont universels et transposables sur d'autres logiciels tel que Blender, 3dsMax etc

## Concepts clés 

- Vous pouvez accomplir 95% du travail avec quelques outils identiques. Maîtrisez les outils de modélisation de base et gardez les choses simples.

- Une bonne référence rend tous les modèles plus faciles à réaliser.

- Travaillez à l'échelle du monde réel. Cela facilite la modélisation.

- Les triangles et les Ngons ne sont pas mauvais si vous comprenez comment travailler avec eux.

- Vous pouvez modéliser presque tout à partir de simples primitives. Essayez de démarrer tous les modèles à partir de formes simples.

- Gardez les modèles combinés ou séparés selon leur état dans le monde réel. Ne modélisez pas tout sous une seule forme s'ils sont séparés dans le monde réel.

## Blocs de construction d'un mesh

Tous les modèles ou "mesh" se composent de sommets (Vertices), d'arêtes (Edges), de polys (Faces).

La manière dont vous modélisez consiste à manipuler (déplacer, redimensionner et tourner) ces blocs de construction ou à en ajouter davantage. Le reste concerne comment faire cela plus rapidement et intelligemment. Nous avons aussi trois principaux types de polygones : Triangle (3 sommets), Quad (4 sommets) et Ngon (plus de 4 sommets).



<iframe width="1920" height="720" src="https://www.youtube.com/embed/-bZ7gstIWyI" title="The Polygon" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe width="1920" height="720" src="https://www.youtube.com/embed/VXS70tRhMb8" title="Multisided Polygon" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


Tout est fait de triangles en interne:

#TODO image d'illustration

Ici nous avons afficher les triangles de face à droite (Menu Display > Polygons > Face Triangle)

## Modeliser à l’échelle

Il est très important de commencer par ajouter un personnage dans votre scène et de vérifier dans quelle unité vous modélisez.
Par défaut Maya est en cm mais vérifiez que c'est bien le cas malgré tout

Utilisez le content browser pour ajouter un personnage dans votre scène.

Il y a deux raisons principales pour lesquelles vous voulez travailler à l'échelle du monde réel :

- Collaboration : il est bien plus simple de travailler ensemble si on modélise à l’echelle.

- Les lumières et les matériaux réagissent de manière fiable.

Définir votre scène en cm

Windows > Settings- Preferences > Preferences >Setings :

Linear : cm/m

Angular : degrees

#TODO image d'illustration


## Outils de Sélection


- Retirer de la sélection - Clic Ctrl

- Inverser - Glisser Shift LMB - Inverser - Maj Shift I

- Sélectionner les éléments connectés - Double-cliquez sur le polygone

- Boucle (Loop) - Double-cliquez sur la boucle

- Anneau (Ring) - Double-cliquez sur l'anneau

- Sélection par plage - Sélectionnez le début, double-cliquez sur le point de fin

- Menu de sélection (Selection Pie Menu) - Ctrl RMB

- Désélectionner tout - Alt D

- Agrandir la Sélection - Shift >

- Réduire la Sélection - Shift <

## Utilisation des "Marking menus” dans Maya

Vous pouvez effectuer presque toute la modélisation en utilisant uniquement "Marking menus”. Combinez-les avec quelques raccourcis personnalisés et vous serez imbattable.

- Outils de selection- Clic droit

- Outils de modélisation - Ctrl + Shift + Clic droit

- Outils de sélection - Ctrl + Clic droit

Les menus sont basés sur des gestes et vous pouvez glisser dans la direction de la fonctionnalité que vous souhaitez - pas besoin d'attendre que le menu s'ouvre. Les menus de marquage sont également basés sur le contexte : vous obtenez différents outils selon que vous soyez en mode Objet, Sommet ou Bordure.

# Outils de Modélisation

Extrusion : Ajoute plus de géométrie en extrudant une face ou un sommet. Utilisez Shift + Clic gauche avec soit l'outil de déplacement, de redimensionnement ou de rotation pour extruder facilement.

Insertion : Ajoute plus de géométrie en insérant une face. N'ajoute pas de hauteur car il travaille avec la forme que vous avez déjà.

Biseau (Bevel) : Parfait pour ajouter des triples bords à vos modèles, ou pour ajouter des courbes aux modèles. Principalement utilisé sur les bords.

Ajustement (Tweak) : Vous permet de déplacer rapidement les sommets.

Dupliquer : Utilisez Ctrl + D ou maintenez la touche Shift enfoncée tout en déplaçant pour dupliquer votre modèle.

Séparer (Separate) : Sépare chaque pièce détachée en son propre maillage.

Fusionner (Merge) : Fusionne les sommets.

Pont (Bridge) : Ajoute des polygones entre les bords sélectionnés.

MultiCut : Utilisé pour découper la topologie dans un polygone. Maintenez la touche Ctrl enfoncée pour ajouter des boucles.

Edge Slide : Déplace les bords sur une surface sans modifier la topologie.

Insert Edge Loop : Utilisé pour ajouter des boucles de bord. Dans les paramètres de l'outil, vous pouvez ajouter plusieurs boucles en même temps.

Lisser (Smooth) : Subdivise le modèle en augmentant le nombre de polygones par 4. Cela diffère de l'utilisation de la touche 3 car cela ajoute réellement la topologie à votre modèle.

Fill Hole : Remplit les trous où les bords sont sélectionnés. Vous n'avez besoin de sélectionner qu'un seul bord du trou." et non pas toute la boucle de bord. Trianguler : Transforme le modèle en triangles.

## Détachement et combinaison

Si vous travaillez sur des parties d'un modèle séparément, vous pouvez les détacher pour travailler dessus. Après avoir terminé, combinez-les pour former un seul maillage.

Outils :

• Mesh - Detach

• Mesh - Combine

## Manipulateur et Pivots

Un pivot est le point à partir duquel la rotation, la translation ou la mise à l'échelle se produisent.

• Aligner le Pivot - Maintenez D enfoncé - ou Insert et cliquez sur une face, un sommet ou un bord.

• Centrer le Pivot : Modifier - Centrer le Pivot

(Parler de l’axis orientation , pivot custom, bake pivot etc)

## Dépliage UV

Projection Workflow

Couture Unfold Workflow

Texture unique, teture Tile

Videos : https://www.youtube.com/watch?v=dj0uXid9oGo&list=PLBX-X8mPyxIqdD00QnDXRDzENfS0_l1vW

## Vertex Normals

## Bases des Curves

- Créer - Outils de courbe

- Bézier - polyvalent.

Cliquez pour des courbes droites

• Cliquez +"

Sweep Mesh

Sweep Mesh est un outil de modélisation qui rend les courbes bien plus puissantes et flexibles. Les formes sont UVées, vous pouvez changer la courbe de base à tout moment et le nombre de sections peut être modifié interactivement.

Video : https://www.youtube.com/watch?v=6RIHSfW5x2Q

Déformeurs

Les déformeurs vous permettent de déformer vos modèles de manière non-destructive. Lattice - Crée une forme de treillis que vous pouvez utiliser pour déformer le maillage. Utile pour de grands changements sur un modèle. Non-Linéaire :

• Plier - Plier le modèle.

• Torsion - Tord le modèle

• Évasement - Réduit le modèle

• Texture - Déforme le modèle à l'aide d'une carte de texture ou d'une procédure.

Modélisation SubD

Si vous voulez que vos modèles semblent plus réalistes, vous devrez probablement subdiviser vos modèles, car sinon, ils seraient bien trop anguleux. Ceci utilise une méthode appelée surfaces de subdivision (SubD).

• Polygones - 1

• Cage - 2

• Lisse - 3

Changer le niveau de subdivision de la preview:

• Shape Node – Subdivision Levels - Preview Division Levels

Conseils

Ne modélisez pas avec SubD actif. Cela déforme beaucoup la forme de base, au point qu'elle aura une apparence complètement différente de la version SubD. Les animateurs et les riggers travailleront uniquement avec le modèle non-SubD, donc le modèle poly brut doit être propre. Vous n'avez pas à tout modéliser pour SubD. C'est beaucoup plus lourd à rendre et plus difficile à modéliser.

Modéliser en une seule pièce ou en plusieurs pièces ?

Modélisez en fonction de la manière dont l'objet est construit dans la réalité. S'il est combiné en une seule forme, faites-le en une seule forme. Si c'est séparé, séparez les pièces. Il est généralement bien meilleur de modéliser séparément :

• BEAUCOUP plus facile à modéliser

• Plus réaliste

• Plus facile à manipuler et à déformer

Comment tout modéliser

Démontez chaque forme en formes simples. Utilisez la géométrie de base comme point de départ :

• cube

• sphère

• cylindre

• tore (donut)

• plan

Qu'est-ce qu'une bonne topologie ?

La topologie fait référence à la distribution et à la structure des bords d'un modèle 3D. La topologie est un moyen d'optimiser nos modèles pour la performance, la déformation - ou les deux. Une bonne topologie est celle qui fait le travail! Ne vous laissez pas prendre par une topologie visuellement plaisante. C'est une technique d'optimisation technique et il n'y a pas toujours de lien entre ce qui semble bon et ce qui est bon.

Raccourcis clavier

Personnalisez votre espace de travail en créant des raccourcis clavier pour les fonctions que vous utilisez fréquemment. Cela accélère considérablement le processus de modélisation.

Windows - Paramètres/Préférences - Éditeur de raccourcis

• Isoler Basculer - Alt Q

• Basculer Rayon X Objet - Alt Z

• Basculer Rayon X Scène - Shift Alt Z

• Fusionner les Sommets - Shift X

• Centrer le Pivot - Ctrl Alt Q

• Multi-Coupe - Alt C

• Soudure Ciblée - Shift V

• Glisser"

"outil de glissement de bord - Shift S

• Pont - Shift B

• Connecter - Z

• Affichage/Masquage de la grille - Shift G

• Inversion de la sélection - Alt 2

• Éditer le flux de bord - Alt A

Utilisation des sets de sélection

Les sets de sélection vous permettent de sélectionner rapidement des groupes prédéfinis de vertices, edges ou faces. Cela est particulièrement utile pour les modèles complexes.

Créer un set de sélection :

• Sélectionnez les composants souhaités > Edit - Quick Select Set

Layers (Couches)

Organisez votre scène en utilisant des couches. Cela vous permet de cacher, afficher ou rendre sélectif des parties de votre scène.

Layer Editor :

• Créez une nouvelle couche

• Assignez des objets à une couche

Réflexions sur la modélisation

Modéliser est autant un art qu'une science. Il est important de prendre le temps d'apprendre les bases, mais aussi d'expérimenter et de trouver votre propre flux de travail. Soyez patient, pratiquez régulièrement et n'hésitez pas à demander de l'aide ou des critiques.

Corriger les erreurs de modélisation courantes

Utilisez l'outil de nettoyage pour corriger de nombreuses erreurs courantes :

Géométrie non-manifold (non manifold geo).

Faces lamina (Lamina faces).

Faces avec une zone de mappage nulle (non UVé).

Soyez attentif à :

Les UVs qui dépassent d'une tuile.

Les triangles.

Les Ngons.

Les formes désordonnées.

Les normales inversées.

Remarque : Si vous avez des zones qui sont vraiment endommagées, il est généralement beaucoup plus rapide et facile de supprimer la mauvaise zone, puis de la remodeler.
 