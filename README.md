# Gradient Descent Visual Lab

Ce projet pédagogique aide à comprendre et à visualiser le **gradient** ainsi que les méthodes d'optimisation fondées sur celui-ci.

L'objectif n'est pas seulement d'exécuter un algorithme, mais d'observer graphiquement :

- la direction indiquée par le gradient ;
- le déplacement produit par la descente de gradient ;
- l'influence du taux d'apprentissage ;
- la différence entre un minimum local et un minimum global ;
- l'importance du point de départ ;
- le passage d'une courbe en 2D à une surface en 3D ;
- le lien entre l'optimisation mathématique et le machine learning.

## Principe étudié

Le gradient indique la direction dans laquelle une fonction augmente le plus rapidement. Pour faire diminuer la fonction, la descente de gradient se déplace dans la direction opposée :

$$
\theta_{k+1}=\theta_k-\alpha\nabla f(\theta_k)
$$

où :

- $\theta_k$ représente la position actuelle ;
- $\nabla f(\theta_k)$ représente le gradient à cette position ;
- $\alpha$ représente le taux d'apprentissage ;
- $\theta_{k+1}$ représente la nouvelle position.

## Progression pédagogique

Chaque notebook introduit une difficulté supplémentaire.

| Notebook | Dimension visualisée | Notion principale |
|---|---|---|
| 01 — Courbe convexe | 2D | Pente, dérivée et minimum global |
| 02 — Fonction non convexe | 2D | Minimums locaux, maximums locaux et initialisation |
| 03 — Taux d'apprentissage | 2D | Convergence lente, oscillation et divergence |
| 04 — Surface à deux variables | 3D | Gradient vectoriel et courbes de niveau |
| 05 — Points critiques | 3D | Minimum, maximum et point selle |
| 06 — Montée de gradient | 2D et 3D | Recherche d'un maximum |
| 07 — Régression linéaire | Machine learning | Minimisation d'une fonction d'erreur |

## Comprendre les dimensions

### Visualisation 2D

Une fonction d'une variable,

$$
y=f(x),
$$

est représentée par une courbe. Le gradient correspond alors à la dérivée $f'(x)$, c'est-à-dire à la pente locale.

### Visualisation 3D

Une fonction de deux variables,

$$
z=f(x,y),
$$

est représentée par une surface. Son gradient devient un vecteur :

$$
\nabla f(x,y)=
\begin{pmatrix}
\dfrac{\partial f}{\partial x} \\
\dfrac{\partial f}{\partial y}
\end{pmatrix}.
$$

La trajectoire de l'algorithme sera observée à la fois sur la surface 3D et sur une carte de courbes de niveau.

## Méthode utilisée dans les notebooks

Chaque notion est étudiée dans le même ordre :

1. intuition mathématique ;
2. définition de la fonction ;
3. calcul du gradient ;
4. calcul manuel d'une mise à jour ;
5. code Python commenté ;
6. visualisation de la trajectoire ;
7. modification des paramètres ;
8. interprétation du résultat ;
9. exercice progressif.

## Technologies

- Python ;
- NumPy pour les calculs numériques ;
- Matplotlib pour les visualisations 2D et 3D ;
- Jupyter Notebook pour combiner les explications, le code et les graphiques.

## Objectif final

À la fin du projet, il devra être possible d'expliquer visuellement pourquoi un algorithme :

- se dirige vers une certaine région ;
- atteint parfois seulement un minimum local ;
- dépend de son initialisation et de son taux d'apprentissage ;
- peut osciller, diverger ou rester près d'un point critique ;
- permet d'entraîner un modèle de machine learning en minimisant son erreur.

Ce projet fait partie de la préparation au cours **IFT 6390**.

Ce petit Lab à été réaliser par un **ETUDIANT** je peux me tromper !
