# Curso de Git y Github

---

<details><summary> <b>Conceptos de Git y Github</b></summary>

## Que es git

>Es un controlador de versiones este es un sistema que registra cada
>cambio que se realiza en el código fuente de un proyecto. Esto
>te permite tener un histórico de todos los cambios producidos
>en sus ficheros, saber quién lo hizo y cuándo.

## Los 3 estados de git
* Modified: Es cuando un archivo ha sido creado, eliminado o modificados.
* Staged: Es cuando el archivo ha sido marcado como  preparado para ser confirmado en el repositorio local.
* Commited: Es cuado el los archivos marcados como preparados son subidos al repositorio local.

![3 tipos de estados](/img/image.png)

## Que es el head
>El head es basicamente decirte estoy aqui.

## Que es un commit
>Son como un punto de guardado como en un videojuego.

## Que es una rama

>Una rama es un snapshot de la division del codigo, en otras palabras son apuntadores que apuntan a un commit.

![ramas](/img/image-1.png)

## ¿Git y GitHub son lo mismo?

>Respuesta corta no, git es un controlador de versione encambio github es servicio de alojamiento en la nube de código fuente basado en el sistema de control de versiones(git).

![git_vs_github](/img/image3.png)

## Fusionar ramas
>La fusion de dos ramas es cuando integramos los cambios de una rama a otra.

## Porque eliminar una rama?
>Porque es una buena practica ademas se mantiene limpio el espacio de trabajo

## Conflictos en git
>Un conflicto en es cuando git no sabe que cambio debe prevalecer posterior a un merge, lo que requiere que lo resolvamos manualmente.

![conflicto](/img/image2.png)

## Dentro de github podemos encontrar lo siguiente

* Ver mi perfil y mis repositorio: Podemos ver nuestra información de nuestro perfil, repositorios, organizaciones a las que pertenecemos y ver nuestras contribuciones.
* Buscar perfiles, repositorios , etc.: Podemos ver nuestros repositorios y repositorios de otras personas.
* Proyectos: Nos permite ver, crear y gestionar proyectos.
* Organizaciones: Nos permite crear repositorios privados y poder agregar personas a este.
* Repositorios y codigo: Podemos ver archivos de los repositorios publicos y personales, se puede realizar cambios en el código.
* Acciones en los repositorios: Las actions nos permiten automatizar las tareas en nuetro repositorio.

### Para usar un repositorio remoto debemos hacer lo siguiente
* Crear una cuenta en GitHub
* Crear un repositorio local en nuestro ordenador.
* Vincular el repositorio local con el repositorio remoto en GitHub
* Sicronizar nuestros cambios del repositorio local con el repositorio remoto

## Push, pull y pull request

### ¿Que es git push?

>Es un comando que nos permite subir los cambios de nuestro repositorio local a nuestro repositorio remoto. Este se asocia a solo una rama.

### ¿Que es git pull?
>Es un comando que nos permite descargar los cambios de nuestro repositorio remoto a nuestro repositorio local.

### Malas prácticas del git push
>El git push -f o git force push, es una mala práctica porque puede sobreescribir los cambios de otros usuarios en el repositorio remoto.

### Como crear un pull request o PR
>Un pull request es una solicitud de revision y fusión de los cambios de una rama en otra rama que son enviados al repositorio original. Un pull request se puede crear desde la plataforma de GitHub o desde la linea de comandos de git. Se puede hacer pull request con commits pequeños y poder visualizarlos, esto cuenta como una buena práctica.

</details>

---

# Comandos utilizados
| Comando                     | Descripción                                                                |
| -------------------------   | -----------------------------------------------------------------          |
| **git init nombre_proyecto**    | Inicia un nuevo repositorio Git.                                           |
| **git status**                | Muestra el estado actual del proyecto.                                     |
| **git add**                   | Agrega todos los archivos al repositorio de Git.                           |
| **git restore --staged**      | Evita que los cambios en el área de preparación se incluyan en el commit.  |
| **git commit**                | Genera un registro del cambio realizado.                                   |
| **git log**                   | Muestra un historial de los commits realizados.                            |
| **git log --online**                   | Muestra un historial de los commits realizados pero la parte que se se hizo commit sin tanto detalle.                            |
| **git commit -amend-m**       | Permite editar el mensaje del commit.                                      |
| **git branch**               | Nos muestra todas las ramas del repositorio actual.                        |
| **git branch rama_nueva**  | Crear una rama este tiene diferentes complementos.                         |
| **git switch rama_nueva**  | Permite cambiar de una rama a otra en nuestro repositorio local.            |
| **git switch -c rama_nueva**  | Permite crear y cambiar de una rama a otra en nuestro repositorio local.            |
| **git checkout rama_nueva**| Cambia la ubicación actual al "nombre_rama" con todos los cambios.         |
| **git branch -a**            | Permite ver a las ramas locales y remotas.                                 |
| **git branch -d rama_nueva**            |Elimina una rama local, solo si ya ha sido fusionada (merged) con tu rama actual o con la rama main.  |
| **git branch -D rama_nueva**            | Es una eliminación forzada.                  |
| **git merge**            | Fusiona los cambios de una rama con otra rama.                  |
| **git diff**            | Sirve para visualizar las modificaciones en los archivos|