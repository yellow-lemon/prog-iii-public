# Processus de compilation
![](img/processus-de-compilation.png)

# Creation de libraries
![](img/creation-de-library.png)
```ps
gcc -c ./Addition.c
ar -rcs ./libAddition.a ./Addition.o
```

```ps
gcc ./main.c -o Programme.exe -L. -lAddition
```

# Documentation
Fichier : 
```
/// \File nomFichier.ext
/// \Author Prenom Nom (courriel)
/// \brief description
```

Fonction :
```
/// \Brief description
/// \Param identificatuer description
/// \return descripiton
```