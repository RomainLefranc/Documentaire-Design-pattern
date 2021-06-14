# Documentaire-Design-pattern

## Singleton

Singleton est un patron de conception de création qui garantit que l’instance d’une classe n’existe qu’en un seul exemplaire, tout en fournissant un point d’accès global à cette instance.

Il garantit l’unicité d’une instance pour une classe

Toute mise en place d’un singleton est constituée des deux étapes suivantes :

Rendre le constructeur par défaut privé afin d’empêcher les autres objets d’utiliser l’opérateur new avec la classe du singleton.
Mettre en place une méthode de création statique qui se comporte comme un constructeur. En sous-main, cette méthode appelle le constructeur privé pour créer un objet et le sauvegarde dans un attribut statique. Tous les appels ultérieurs à cette méthode retournent l’objet en cache.
Si votre code a accès à la classe du singleton, alors il peut appeler sa méthode statique. À chaque appel de cette méthode, c’est toujours le même objet qui est retourné.

### Objectifs : 

- Assurez-vous qu’une classe n’a qu’une seule instance et fournissez un point d’accès global.

La classe est statique
Les accesseur sont statiques
le constructeur de la classe est private
l’objet est uniquement initialisé la première fois qu’il est appelé.

## Private Class Data

Le modèle de conception des données de la classe privée vise à réduire l’exposition aux attributs en limitant leur visibilité.

Il réduit le nombre d’attributs de classe en les encapsulant dans un seul objet Data. Il permet au concepteur de classe de supprimer le privilège d’écriture des attributs qui sont destinés à être définis uniquement pendant la construction, même à partir des méthodes de la classe cible.

### Objectifs

- Contrôler l’accès en écriture aux attributs de classe
- Séparer les données des méthodes qui les utilisent
- Encapsuler l’initialisation des données de classe

Bloquage de l'accès direct aux attributs d'un objet
Tout les attributs sont private
Obligation d'utiliser des setter / getter pour interagir avec les données
 
## State

État est un patron de conception comportemental qui permet de modifier le comportement d’un objet lorsque son état interne change.

Le patron de conception état propose de créer de nouvelles classes pour tous les états possibles d’un objet et d’extraire les comportements liés aux états dans ces classes.

Ajout d'une classe state permettant de données a une class un état pouvant changé 


