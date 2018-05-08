## DEGATS
Une figurine est toujours dans un des trois niveaux de Dégâts suivants :
+ **Indemne** : L’état initial d’une figurine lors du déploiement.
+ **Blessée** : La figurine continue de se battre. Elle subit des pénalités pour quelques tests, mais reste néanmoins capable de continuer à agir normalement.
+ **Morte** : La figurine est retirée du jeu.

### Résoudre les Dégâts.
Chaque attaque réussie génère un nombre de _**Dégâts Potentiels**_.

Les Dégâts Potentiels peuvent être également provoqués par des évènements, tels qu’une chute ou une projection contre un mur.

Les effets de tout Dégât Potentiel sont résolus comme suit :
1. L’Armure de la figurine ciblée est réduite par la valeur PA de l’attaque, jusqu’à un minimum de 0.
2. L’Armure restante de la figurine ciblée (si elle en a une) est soustraite des Dégâts Potentiels pour calculer les _**Dégâts Effectifs**_.
3. Ces Dégâts Effectifs sont ajoutés à tous les Dégâts précédemment subis et comparés à la Taille de la figurine, en se référant au tableau en bas de page pour déterminer les effets.

#### Exemple :
> Une figurine Indemne de Taille 1 est touchée par une attaque provoquant 2 Dégâts Potentiels. En consultant le tableau, nous pouvons voir que cette attaque tuerait une figurine de cette Taille non-protégée par une armure. «Heureusement», la figurine porte une Armure 1. Celle-ci réduit les Dégâts Effectifs de 1 point, et la figurine est simplement Blessée.  
> Si l’attaque bénéficiait de la capacité PA1, l’unique point d’Armure aurait été pénétré, décompté, et la figurine serait Morte.

#### Calculs :
```
Armure Effective = Armure - PA  
Dégats Effectifs = Dégats Potentiels - Armure Effective
```

### Tableau d'application des dégâts
|Dégâts totaux de la figurine  (y compris les précédents Dégats subis)|Effets|
|---|---|
|**0 Dégat**|La figurine est _Indemne_|
|**1 Dégât ou plus, mais pas plus que la Taille de la figurine.**|La figurine est _Blessée_. Marquez la figurine avec un nombre de Pions de Dégâts équivalent au nombre de Dégâts Effectifs provoqués.|
|**Plus de Dégâts que la Taille de la figurine.**|La figurine est _Morte_. Retirez-la du jeu.|

