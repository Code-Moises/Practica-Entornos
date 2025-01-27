# Procedimientos Básicos para Ramificar y Fusionar en Git

Este repositorio presenta un ejemplo de cómo trabajar con ramas y fusionarlas en **Git**. A través de este ejercicio, se simula un flujo de trabajo común en desarrollo de software, que incluye la creación de ramas para nuevas funcionalidades y la resolución de problemas urgentes mediante ramas de corrección (`hotfix`). Este flujo es utilizado para mantener un flujo de trabajo limpio y organizado sin perder ningún cambio importante.

## Descripción

En este ejercicio, se siguen los siguientes pasos básicos:

1. **Creación de una rama de trabajo**: Se crea una rama para trabajar en una nueva funcionalidad o tarea (por ejemplo, el problema #53).
2. **Cambio a una rama de producción**: Si surge un problema urgente en producción, se cambia a la rama principal (`master`) y se crea una rama para solucionar dicho problema (por ejemplo, `hotfix`).
3. **Fusión de ramas**: Después de solucionar el problema, se fusiona la rama de corrección (`hotfix`) de nuevo en la rama principal. Posteriormente, se vuelve a la tarea original y se continúa trabajando en ella.
4. **Finalización del trabajo**: Una vez que el trabajo en una rama se completa, se fusiona nuevamente en la rama principal y se elimina la rama utilizada para la tarea.

Este flujo de trabajo es útil para garantizar que los desarrolladores puedan solucionar problemas urgentes sin perder el progreso que ya han hecho en otras tareas.

## Pasos Realizados

1. **Creación de ramas**:
   - Se creó una rama `iss53` para trabajar en el problema #53.
   - Luego, se cambió a la rama `master` para crear una rama `hotfix` y resolver un problema urgente.

2. **Fusión de ramas**:
   - Después de resolver el problema en la rama `hotfix`, se fusionó con la rama `master`.
   - Finalmente, se volvió a la rama `iss53` y se completó el trabajo pendiente.

3. **Eliminación de ramas**:
   - Las ramas `hotfix` y `iss53` fueron eliminadas después de completar el trabajo correspondiente.

4. **Manejo de conflictos**:
   - En el caso de que haya conflictos durante una fusión, se resolvieron manualmente o utilizando herramientas de resolución de conflictos como `git mergetool`.

## Comandos Utilizados

* **Crear una nueva rama**:
  *git checkout -b <nombre_rama>*
  
* **Cambiar de rama:**
    *git checkout <nombre_rama>*

* **Confirmar cambios (commit):**
    *git commit -a -m "Descripción del cambio"*

* **Fusionar una rama con la rama actual:**
    *git merge <nombre_rama>*

* **Eliminar una rama:**
    *git branch -d <nombre_rama>*

* **Verificar el estado de las ramas:**
    *git status*

* **Resolver conflictos con herramientas de fusión:**
    *git mergetool*


## Resolución de Conflictos

En caso de que se presenten conflictos durante una fusión, Git marcará los archivos conflictivos y te pedirá que resuelvas las diferencias manualmente. Los conflictos pueden ser resueltos editando los archivos directamente y utilizando los comandos git add y git commit para finalizar el proceso.
