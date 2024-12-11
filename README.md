# Summative-4FSC0PF001-Resubmissiom
## Pirate Game : collect the treasures

Creer un jeu dans lequel vous pilotez un bateau pirate et vous chercherz à ramasser un certain nombre de trésors.
## Regles du jeu
  - Si le bateau se superpose à un trésor, le trésor disparait et le score augmente d'un nombre aléatoire 
  - Une fois tous les tresors collectés, on fait reappaitre les tresors a des emplacements differents et le chrono est relance.
  - A chaque nouvelle apparition des tresors, il y a de plus en plus de tresors
  - A chaque nouvelle apparition des tresors, le chrono est relance
  - Si le chronometre aarrive à 0, la partie s'arrete

## Contraintes
- Creer une classe **Game** pour gerer l'affichage des differents elements, et assurer le respect des regles du jeu
  - Elements à afficher
    - Tresors
    - Bateau
    - Score
    - Chronometre
    - Mer
- Creer une classe **PirateShip** pour piloter le bateau avec les combinaisons de touche suivante : touches directionelles ou WASD
  - Les touches **Haut/Bas** pour avancer
  - Les touches **Gauche/Droite** pour faire pivoter le bateau
- Creer une classe Treasure pour gerer les fonctionnalites suivantes
  - Afficher les tresors
  - Permettre la collecte de ces tresor
  - Determiner le score attribuer à chaaue tresor  



## Informations
Pour appliquer une rotation, et faire bouger le bateau *vers l'avant* :

``` c++
// Forward direction (local +x direction in global space)
float angleRad = sprite.getRotation() * (3.14159265358979323846f / 180.0f);
sf::Vector2f forward(std::cos(angleRad), std::sin(angleRad));
```
