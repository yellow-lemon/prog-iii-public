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

boot-repair