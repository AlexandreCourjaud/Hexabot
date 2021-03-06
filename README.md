# Hexabot

Ceci est le dépôt Git pour le cours d'ingénierie système et modélisation robotique de l'UV 5.8 à l'ENSTA Bretagne en 2020.


## Lancer la simulation

### Dépendences

- ros-melodic-effort-controllers  # contrôleur  
- ros-melodic-hector-mapping      # positionnement
- cv2  (version 3.2.0 testée)     # traitement d'image  
- numpy                           # calcul  
- matplotlib                      # affichage simple  
- scikit-image                    # traitement d'image  

### Démarrer la simulation

Pour lancer l'exploration de la grotte, repérage des failles et visualisation incluses:

```bash
roslaunch phantomx_mapping exploration.launch
```  

Alternativement, pour une version démo:
```bash
roslaunch phantomx_gazebo phantomx_gazebo.launch
```
puis lancer demo walker.py

```bash
rosrun phantomx_gazebo demo_walker.py
```


## Groupe

### Membres

Yann Musellec  
Corentin JEGAT  
Alexandre Courjaud  
Matthieu Bouveron  
Philibert ADAM  
Driss Tayebi  

### Gestion de projet
Pour la gestion du projet séance par séance, nous utilisons [taiga](https://tree.taiga.io/project/erysme-hexapode_nom_groupe/)


## Structure du dépôt

### Workspace ROS

Le dossier `workspaceRos` est la racine du workspace `catkin` pour les packages ROS. Ces derniers sont placés sous `workspaceRos/src`.    
Consulter le [README](workspaceRos/README.md) du workspace pour plus d'informations.


### Documents

Le dossier `docs` contient tous les documents utiles au projet:
- Des [instructions pour utiliser Git](docs/GitWorkflow.md)
- Un [Mémo pour ROS et Gazebo](docs/MemoROS.pdf)


### Rapports

Le dossier `reports` contient les rapports d'[objectifs](reports/GoalsTemplate.md) et de [rétrospectives](reports/DebriefTemplate.md) en suivant les deux templates mis à disposition. Ces deux rapports sont rédigés respectivement au début et à la fin de chaque sprint.
