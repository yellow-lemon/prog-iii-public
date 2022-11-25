# Pointeur
## Description 
Variable qui contient une adresse de la mémoire centrale, plutôt qu'une valeur.

## Déclaration
```cpp
int entier;
int* pEntier;
```
![](img/pointeur-declaration.png)

## Allocation
```cpp
pEntier = new int; //Équivalent du malloc
```
**Attention :** Lorsqu'il y a un new, il doit y avoir un [delete](#déréférencement)

![](img/pointeur-allocation1.png)
```cpp
entier = 3;
*pEntier = 5;
```
![](img/pointeur-allocation2.png)

## Indirection
```cpp
*pEntier = 43;
```
![](img/pointeur-indirection.png)

## Déréférencement
```cpp
pEntier = &entier; // Le & permet d'obtenir l'adresse d'une variable
```
![](img/pointeur-dereferencement.png)

## Libération
```cpp
delete pEntier;
```
La libération de mémoire n'initialise pas à zéro (opération inutile), elle libère l'espace réservé.

## Pointeur null
`nullptr` pointe sur l'adresse 0
```cpp
pEntier = nullptr;
```
![](img/pointeur-nullptr.png)

# Exemple
## Exemple 1 (Allocation et libération)
![](img/pointeur-exemple1.png)

## Exemple 2 (Déréférencement)
![](img/pointeur-exemple2.png)

