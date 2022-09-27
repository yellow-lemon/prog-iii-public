## ENTIER
- char : 1 octet
- short : 2 octets
- int : 3 octets
- long : 4 octets

peuvent être unsigned

## RÉELS
- Float 4 octets
- Double 8 octets

## DÉCLARATION DE VARIABLES
Type indicateur;
- Débute tjrs par une lettre ou un tiret (-)
- Contient que des lettres, chiffres, et tiret (-)
- Pas de terme qui existe dans le language (example : if)

```c
int entierA, entierB, entierC;
int entier1 = 12, entier2;
```

## TABLEAU
Type identificateur[N];
```c
int tabEntiers[5];
```
### String 
char chaine[N + 1] La dernière case doit toujours être zéro

## POINT D'ENTRÉE
```c
int main() {
    return 0;
}
```
ou
```c
int main(int argc, char* argv[]) {
    return 0;
}
```
ou
```c
void main() {
    return 0;
}
```

## MACRO
### Define
(rechercher remplacer)
```c
#define IDENTIFCATEUR (constante)
#define PI 3.14159
#define TPS 5
#define TVQ 9.975
```


### Include
```c
#include <nomFichier ext> // Bibliothèque système
#include "nomFichier.ext" // fichier de projet

(copier coller)
```

### FRAGMA ONCE
```c
#fragma once //Inclure une seul fois
```
```c
#ifndef HEADER_H
#define HEADER H
```

## Définition de type
```c
typedef unsigned char byte;
```

## Oprérateurs
Arithmétiques : =, +, -, *, /, %, ++, -- \
relationels : ==, <, <=, >, >=, != \
logique :
- bitwise : |, &
- logique : ||, &&

incrémentation
```c
int i = 0;

++i; //pre
i++; //post
```

## IF
```c
if (condition) {
    instructionA();
}
else {
    instructionB();
}
```

## Switch
```c
int i = 4;

switch(i) {
    case 1:
        instructionA();
        break;
    case 4:
        instructionB();
    case 5:
        instructionC();
        break;
    case 6:
        instructionD();
        break;
}
```
Le break permet de sortir du case, donc ici, puisqu'il n'y a pas de break dans le case 4, instructionC() sera aussi exécuté
## Structure de répétition
tant que :
```c
while (condition) {
    instructionA();
    instructionB();
}

do {
    instructionC();
    instructionD();
} while (condition);
// Différence avec le while : Le do while s'exécute au moins une fois même si la condition est fausse
```
pour
```c
for (initialisation; condition; postitération) {
    conditionA();
}

for (int i = 0; i < 42; i++) {
    conditionA();
}

```
## gcc
`gcc main.c`
`gcc main.c -o programme.exe`
`gcc -g main.c`
