# Práctica del curso de Git, GitHub y Sourcetree
## Josep Miquel Arenas Beltran
### Junio del 2021

** ¿Qué comando utilizaste en el paso 11? ¿Por qué? **
- `git reset –hard HEAD~1`.
- `git reset` es el comando que revierte los cambios de un commit para volver a uno anterior y mover el head. Además, le añadimos la instrucción `–hard`, un parámetro que indica que también se deben deshacer los cambios en el working copy y usamos `HEAD~1` para indicar el nombre de commits que deseamos deshacer.

** ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? **
- `git reflog`
- `git reset –hard 23d4267`
- Utilizamos `reflog` para ver el rastro de migas y poder buscar el hash que identifica el commit al que queremos volver. Nuevamente utilizamos el parámetro `–hard` para que los cambios se efectuen en el working copy.

** El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? **
- No se ha causado ningún conflicto porque no intentamos una fusión donde existen archivos que se han modificado en la misma linea.

** El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? **
- A diferencia del paso numero 13, Git ahora sí que ha detectado que estamos intentando fusionar dos ramas donde hemos modificado las mismas lineas de un archivo y él no puede decir por nosotros que código es el correcto. A continuación, debemos solucionar el conflicto manualmente y subir los cambios al repositorio efectuando un commit.

** El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? **
- No se ha causado ningún conflicto porque sólo hemos modificado el archivo git-nuestro.md de la rama styled y la hemos unido a la principal. Como git no ha detectado ningún conflicto ha adaptado esos cambios automáticamente en la rama master.

** ¿Qué comando o comandos utilizaste en el paso 25? **
- git log --graph

** El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? **
- Sí, porque puedo moverme de una rama a otra sin ningún problema en la misma dirección.
	
** ¿Qué comando o comandos utilizaste en el paso 27? **
- `git reflog`
- `git reset ca35e7b`

** ¿Qué comando o comandos utilizaste en el paso 28? **
- `git restore git-nuestro.md`

** ¿Qué comando o comandos utilizaste en el paso 29? **
- `git branch -D title`
	
** ¿Qué comando o comandos utilizaste en el paso 30? **
- `git reflog`
- `git reset –hard ca335e7b`

** ¿Qué comando o comandos usaste en el paso 32? **
- `git reflog`
- `git reset 65adc68`

** ¿Qué comando o comandos usaste en el punto 33? **
- `git reflog`
- `git reset`
