## Pile
Type : L.I.F.O \
Accès : Dessus \
Fonctionalité :
- Empiler (push)
- Dépiler (pop)
- Compte (size)

Représentation :
- SS (tableau représentant la pile)
- SP (indice du tableau de la pile)

## File
Type : FIFO
fonctionnalités : 
- Enfiler (PUSH)
- Défiler (POP)

## Struct
```c
struct Chien {
    char race[30];
    int age; // Une variable de peut pas être initialisé dans une struct
};

struct ArrayStack chien1;

chien1.age = 12;

//...
```
## Pointeur
Adresse en mémoire centrale
```c
int entier; // valeur entière
int* pEntier; // Adresse en mémoire centrale où se trouve une valeur entière

entier = 42;
```
![](img/pointeurdeclaration.PNG)

```c
pEntier = malloc(sizeof(int)); // Pour allouer de la mémoire de X size
```
![](img/pointeurdeclaration2.PNG)
```c
free(pEntier); // Pour libérer la mémoire
```

## Passage des arguments aux paramètres
- Par valeur (copie)
- Par référence
- Par pointeur