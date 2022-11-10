# Include

```cpp
#include <iostream> // Équivalent de stdio.h (pour le cout)
#include <cstdio> // Inclusion bibliothèque C (préfrable de ne pas l'utiliser)
#include <cstdlib> // Pour size_t
```

# Fichiers
- `.cpp` : main
- `.hpp` : En-têtes

# Namespace
```cpp
IntArrayStack::Push(---);
```

Pour ne pas avoir à utiliser le namespace :
```cpp
#include <iostream>
#include <cstdio>
using namespace std;

cout << "entier : " << entier << "PI : " << endl;
// Au lieu de :
std::cout << "entier : " << entier << "PI : " << STD::endl;
```

# Affichage
En c :
```c
int entier = 42;
float PI = 3.1459;
printf("Entier : %i, pi : %f, %f \n", entier, pi);
```

En cpp
```cpp
std::cout << "entier : " << entier << "PI : " << STD::endl;
```

# Types
- **bool**
- **string**

# Pointeur null
```cpp
int *pInt;
pInt = nullptr;
```
`nullptr` pointe sur l'adresse 0

# Limitaion de la pile en C
- Réutilisation --> Fichier d'en-tête
- Plusieurs instances --> Structures
- Limitation/Gaspille de mémoire --> Allocation dynamique et libération
- Robustesse
- Convivialité
- Type imposé

# New
Exemple :
```cpp
Queue<int> fileEntiers = new Queue<int>();
```

1. Instanciation en mémoire
1. Appel du constructeur
1. Retour de l'adresse mémoire de l'instance

## Implémentation
```cpp
Queue<int> fileEntiers = new Queue<int>();
```

// Ajouter une image

```cpp
fileEntier->push(42);
fileEntier->push(404);
```
// Ajouter une image (déja fait)

# Classes
```cpp
class BankAccount {
private : 
  float balance;

public :
  // Constructeur
  BankAccount() {
    balance = 0;
  }
  // Destructeur
  ~BankAccount() {
    delete balance;
  }
  float getBalance() {
    return this.balance;
  }
};
```

## Modification d'accès
- **private** (par défaut) : Accessible que de l'intérieur de la classe.
- **public** : Accessible de partout.
- **protected** : Accessible que de l'intérieur de la classe et de ses classes dérivées.

```cpp
public :
int A;
int B;

private :
int C;
```

## Templates
Au cas où on ne connait pas le type d'avance :
```cpp
template <typename T>

class ArrayStack {
private :
  T* array;
  unsigned long topIndex;
...
```

