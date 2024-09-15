##### - ¿Qué comando utilizaste en el paso 11? ¿Por qué?

```
git reset --hard HEAD~1
```

Para bajar una posición al histórico de commits
##### - ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
```
git reflog
```

Para obtener el identificador del commit, después:

```
git cherry-pick <nº identificador>
```
Para recuperarlo
##### - El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No causa conflicto porque no hay cambios entre las versiones de "main" y "styled"
##### - El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si creó conflicto porque existen variaciones en las mismas líneas de código de una rama a otra. Las ramas "styled" y "htmlify" son ramas que vienen del mismo commit de "main", entonces en cada una de ellas creamos un commit que modifica el archivo en las mismas lineas de código.
Crea conflicto al hacer el merge.
##### - El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No lo ha habido porque "main" estaba más atrasado que el último commit de "styled", etonces lo que hace es aplicar los nuevos cambios de styled en "main"
##### - ¿Qué comando o comandos utilizaste en el paso 25?

```
git log --graph
```
##### - El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Sí podría ser *fast-forward* porque la rama "main" estaba más atrasada que la rama "title"
##### - ¿Qué comando o comandos utilizaste en el paso 27?

```
git reset HEAD^
```
##### - ¿Qué comando o comandos utilizaste en el paso 28?

```
git commit --amend
```

##### - ¿Qué comando o comandos utilizaste en el paso 29?
```
git branch -D title
```
##### - ¿Qué comando o comandos utilizaste en el paso 30?
```
git reflog
```

Para ver el identificador del commit donde hicimos el merge de "main" y "title". Después:

```
git merge <nº de referencia>
```
##### - ¿Qué comando o comandos usaste en el paso 32?
```
git checkout <ref 1er commit>
```
##### - ¿Qué comando o comandos usaste en el punto 33?
```
git checkout main
```
Para volver al último commit de la rama "main"