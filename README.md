# Documentaire-Design-pattern

## Creational patterns

### Singleton

Cas : L'application a besoin de seulement une instance d'un objet.

Singleton est un design pattern de création qui garantit que l’instance d’une classe n’existe qu’en un seul exemplaire, tout en fournissant un point d’accès global à cette instance.

Toute mise en place d’un singleton est constituée des deux étapes suivantes :

- Rendre le constructeur par défaut privé afin d’empêcher les autres objets d’utiliser l’opérateur new avec la classe du singleton.
- Mettre en place une méthode de création statique qui se comporte comme un constructeur.Cette méthode appelle le constructeur privé pour créer un objet et le sauvegarde dans un attribut statique. Tous les appels ultérieurs à cette méthode retournent l’objet en cache.

Si votre code a accès à la classe du singleton, alors il peut appeler sa méthode statique. À chaque appel de cette méthode, c’est toujours le même objet qui est retourné.

Objectifs : 
- Assurez qu’une classe n’a qu’une seule instance et fournir un point d’accès global.

### Prototype

Cas : cloner un objet avec tout ses attributs privé

Prototype est un design pattern qui crée de nouveaux objets à partir d’objets existants sans rendre le code dépendant de leur classe.

Le patron de conception prototype délègue le processus de clonage aux objets qui vont être copiés. Il déclare une interface commune pour tous les objets qui pourront être clonés. Cette interface vous permet de cloner un objet sans coupler votre code à la classe de cet objet. En général, une telle interface ne contient qu’une seule méthode clone.

Elle crée un objet de la classe actuelle et reporte les valeurs des attributs de l’objet d’origine dans le nouveau. Vous pouvez également copier des attributs privés

## Structural patterns

### Private Class Data

Cas : manipulation indésirable des attribut d'une classe.

Private Class Data est un design pattern qui controle l'accès en écriture aux attributs d'une classe

Il réduit le nombre d’attributs de classe en les encapsulant dans un seul objet Data, la visiblité des attributs est limité.

Il permet au concepteur de classe de supprimer le privilège d’écriture des attributs qui sont destinés à être définis uniquement pendant la construction, même à partir des méthodes de la classe cible.

Utilisation de methodes getter et setter pour accéder aux attributs.

Objectifs :
- Contrôler l’accès en écriture aux attributs de classe
- Séparer les données des méthodes qui les utilisent
- Encapsuler l’initialisation des données de classe

## Behavioral patterns

### State

Cas : En fonction de l'etat d'une classe, les methodes n'ont pas le meme comportement.

State est un design pattern qui permet de modifier le comportement d’un objet lorsque son état interne change.

State propose de créer de nouvelles classes pour tous les états possibles d’un objet et d’extraire les comportements liés aux états dans ces classes.

Tout ces états implementeront un interface state, et en fonction du contexte de la classe, la methode utilisé sera differente.








