## Niveles

En el primer nivel, fue algo introductorio me pidio que relizara commit, de tal forma "Git commit" hasta 
un rango de 3 commit.

En el siguiente nivel se utiliza el comando git branch bugFix para crear una nueva rama llamada "bugFix".
Luego, se utiliza el comando git checkout bugFix para cambiarte a la nueva rama "bugFix".

En el siguiente nivel pide crear una nueva rama llamada "bugFix":

- **git branch bugFix** 

Despues cambiar a la rama "bugFix":

- **git checkout bugFix**

Realizar un commit en la rama "bugFix":

- **git commit -m "Fix a bug"**

Volver a la rama "main":

- **git checkout main**

Realizar otro commit en la rama "main":

- **git commit -m "Add new feature to main"**

y por ultimo mergear la rama "bugFix" a "main":

- **git merge bugFix**

En el siguiente nivel pide crear una nueva rama llamada "bugFix" y cambiarse a ella:

git checkout -b bugFix

Realizar un commit en la rama "bugFix":

git add .
git commit -m "Fix a bug in bugFix branch"

Volver a la rama "main" y hacer otro commit:

git checkout main
git commit -m "Add new feature to main"

Volver a la rama "bugFix" y rebasear sobre "main":

git checkout bugFix
git rebase main

El siguiente nivel pide que detacheemos HEAD de bugFix y atacheemosla al commit, en cambio.

Especificá este commit por su hash. El hash de cada commit se muestra en el círculo que lo representa.

- **Se resuelve asi:** git checkout C4

El siguiente nivel pide checkouteá el padre del commit de bugFix. Esto va a detachear a HEAD.

El cual lo resolvi de la siguiente manera, - **Con:** git checkout bugFix^ El símbolo ^ después del nombre de la rama o el hash del commit se utiliza para referirse al commit padre. Esto moverá HEAD al commit padre del último commit en la rama "bugFix".

En el siguiente nivel hacé un rebase interactivo y alcanzá el orden que se muestra en la visualización objetivo. 

En este nivel se usa el comando git rebase -i HEAD~5 y en este aparece un recuadro donde solo debes ordenarlo 
a lo que te pida el nivel.