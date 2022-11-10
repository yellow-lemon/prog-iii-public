# Include

```cpp
#include <iostream> // Équivalent de stdio.h
#include <cstdio> // Inclusion bibliothèque C (préfrable de ne pas l'utiliser)
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
using namespace std;
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
STD::COUT << "entier : " << entier << "PI : " << STD::ENDL;
```

# Types
- **bool**
- **string**

# Limitaion de la pile en C
- Réutilisation --> Fichier d'en-tête
- Plusieurs instances --> Structures
- Limitation/Gaspille de mémoire --> Allocation dynamique et libération
- Robustesse
- Convivialité
- Type imposé

# Classes
```cpp
class BankAccount {
private : 
  float balance;

  // Constructeur
  BankAccount() {
    balance = 0;
  }

public :
  float getBalance() {
    return this.balance;
  }
};
```

# Modification d'accès
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

# Templates