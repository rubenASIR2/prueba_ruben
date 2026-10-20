# Ejercicio 4 colaboración pull request
## Rubén Marcos Cuadrado Ugbomah
## 2º Administración de sistemas informáticos en red 


#### ¿Qué es un pull request?

*Un pull request es una petición que se hace al propietario de un repositorio original para que este último incorpore los cambios que se sugieren*,*En este ejercicio debermos hacer un pull request sobre el siguiente repositorio:https://github.com/lgarciavelazquez/prueba-pr-iaw_202627*

## Lo que vamos a realizar

Realizaremos un *pull request* a este repositorio para solicitar un par de cambios.

## Realización de tareas en mi repositorio local

En mi repositorio local he creado algunos archivos para uso personal, pero posteriormente incluiré todo en la rama nueva correspondiente. Estos son pasos adicionales que estoy siguiendo.

- Modificaremos el fichero `README.md` para añadir un enlace a la lista en el que aparezcan nuestras iniciales.
- El enlace deberá dirigir al fichero que vamos a crear dentro del directorio `files`.
- A continuación, crearemos el directorio `files` y, dentro de él, el fichero `README.md` con el nombre `RMCU`.

* ![Captura1](images/Creación%20del%20directorio%20files.png)

- Crearemos un fichero en el directorio files, que se llame RMCU.md.

* ![Captura2](images/Creación%20del%20markdown%20RMCU.md.png)

*- En el markdown responderemos y a las siguientes preguntas ¿Quienes somos?. ¿Qué asignatura nos gusta más? y ¿Porqué? (debermos utilizar al menos 5 marcas distintas de markdown)

* ![Captura3](images/Archivorcmu.png)

* Versión mejorada
* ![Captura3.3](images/Archivorcmu.version2.0png.png) 


## Realización del *fork* y del *pull request*

Ahora realizaremos un *fork* del repositorio `prueba-pr-iaw` del profesor para crear una copia en nuestra propia cuenta de GitHub. A continuación, clonaremos dicho repositorio en nuestro equipo local para poder trabajar en él.

Una vez clonado, realizaremos los cambios especificados en el enunciado:

- Añadiremos nuestro fichero Markdown al directorio `files`.
- Modificaremos el fichero `README.md` para incluir un enlace a nuestro documento, utilizando nuestras iniciales.
- Confirmaremos los cambios (*commit*) y los subiremos (*push*) a nuestra copia del repositorio.

Por último, crearemos un *pull request* desde nuestra copia del repositorio hacia el repositorio original del profesor (`prueba-pr-iaw`), con el objetivo de solicitar que acepte e incorpore los cambios que hemos realizado.

De esta manera, contribuiremos al repositorio original mediante el flujo de trabajo habitual de GitHub, utilizando *forks* y *pull requests*.

* ![Captura4](images/Fork.png)
* ![Captura5](images/Prueba-pr-iaw%20forkeado.png)

* Clonamos el repositorio 
* `git clone https://TU_USUARIO:TU_TOKEN@github.com/USUARIO/REPOSITORIO.git`
* ![Captura6](images/Clonacióndelrepositoriodeiaw202627.png)


### Creación de una nueva rama de trabajo

Para realizar el Pull Request, creé una nueva rama llamada `ejercicio4-rmcu` en mi repositorio local. De esta manera, puedo trabajar con una rama independiente de `main` y utilizarla para solicitar que el profesor incorpore mis cambios al repositorio original.

En primer lugar, me situé en la rama principal de mi repositorio:

```bash
git switch main
```
* ![Captura7](images/Gitswitchmain.png)
A continuación, creé la nueva rama y cambié a ella mediante el siguiente comando:

```bash
git switch -c ejercicio4-rmcu
```

Para comprobar que la rama se había creado correctamente, ejecuté:

```bash
git branch
```
* ![Captura8](images/Creacionnuevarama.png)

Ahora a continuación pasamos el archivo rcmu a la carpeta iaw202627, e incluimos nuestro enlace.
* ![Captura9](images/pasamoselrmcualpriaw.png)
* ![Captura10](images/Enlaceenfilesrmcu.png)

Después, subí la nueva rama a mi repositorio remoto de GitHub:

```bash
git add
git commit -m "subida del request a rama ejercicio4-rmcu)
git push -u origin ejercicio4-rmcu
```
* ![Captura11](images/gitaddgitcommitgitpushejercicio4-rmcu.png)
* ![Captura12](images/gitpushoriginejercicio4-rmcu.png)

* *Con estos pasos, la rama `ejercicio4-rmcu` quedó disponible en GitHub para realizar el Pull Request*
* *A continuación muestro el estado final de pull request*

* ![Captura13](images/pullrequest.png)
* ![Captura14](images/pullrequest2.png) 


## Aceptación del *pull request* y sincronización del repositorio

Como se puede comprobar, el profesor ha aceptado nuestro *pull request*, por lo que los cambios que propusimos ya se han incorporado al repositorio original.

A continuación, debemos sincronizar nuestra copia del repositorio con la del profesor para incorporar las modificaciones y aportaciones realizadas por nuestros compañeros. De esta manera, mantendremos nuestro repositorio actualizado y tendremos disponibles los cambios que se hayan aceptado mediante los distintos *pull requests*.

Así, todos podremos disponer de una versión actualizada del repositorio, que incluya las contribuciones realizadas por los demás compañeros.

![Captura17](images/1.%20Realización%20de%20la%20sincronizacion.png)
![Captura16](images/1.%20realizacion%20de%20la%20sincronizacion%202.png) 


## Actualización del repositorio local

Una vez sincronizados los cambios en nuestro repositorio de GitHub, el siguiente paso será traer todas esas modificaciones a nuestro repositorio local.

Para ello, ejecutaremos el siguiente comando:

```bash
git pull origin main
```
![Captura19](images/Nos%20traemos%20todos%20los%20cambios%20al%20repositorio%20local.png)