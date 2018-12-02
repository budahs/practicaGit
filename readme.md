#Preguntas ejercicio Git
##¿Qué comando utilizaste en el paso 11?
El comando utilizado ha sido `git reset --hard HEAD~1`.
##¿Por qué?
Ya que sabía que era el commit anterior para usar el HEAD~1 (El número es el número de commits previos). Si no usaría reflog para sacar el id del commit al que quiero establecer el puntero.
##¿Qué comando o comandos utilizaste en el paso 12?
Se han usado `git reflog` y git reset --hard 7aeaab4
##¿Por qué?
El primero para encontrar el id del commit en el qe queremos posicionarnos. El segundo para posicionarnos y ejecutar los cambios en el working copy y recuperar los estilos.
##El merge del paso 13, ¿Causó algún conflicto? 
No me ha dado conflicto.
##¿Por qué?
Porque todos los cambios contenidos en la rama styled estaban contenidos en la rama master.
##El merge del paso 19, ¿Causó algún conflicto? 
Si.
##¿Por qué?
En la rama htmlify se había hecho cambios en el mismo archivo que en la rama styled.
##El merge del paso 21, ¿Causó algún conflicto? 
No.
##¿Por qué?
Porque no había edición del mismo archivo en diferentes ramas. La rama styled contenía todos los cambios de la rama master.
##¿Qué comando o comandos utilizaste en el paso 25?
git log --graph --pretty=oneline
##El merge del paso 26, ¿Podría ser fast forward?
No.
##¿Por qué?
Porque hay cambios en la rama styled que no existían en master.
##¿Qué comando o comandos utilizaste en el paso 27?
git reset HEAD~1
##¿Qué comando o comandos utilizaste en el paso 28?
git checkout -- git-nuestro.md
##¿Qué comando o comandos utilizaste en el paso 29?
git branch -D title
##¿Qué comando o comandos utilizaste en el paso 30?
Primero un git reflog para sacar la referencia de cuando hicimos el merge de title por master y luego `git reset --hard be576b7` para volver al estado y tener los cambios en el working copy
##¿Qué comando o comandos usaste en el paso 32?
Primero git reflog para encontrar la referencia, y luego git checkout 72a21034891a6f401fac430051c794c64d781518 (me entra en estado de HEAD detached pero como iba a volver al estado final me valía sino hubiera usado un reset head) 
##¿Qué comando o comandos usaste en el punto 33?
git reset --hard be576b7
