# Ejercicio 4 colaboración pull request
## Rubén Marcos Cuadrado Ugbomah
## 2º Administración de sistemas informáticos en red 


#### ¿Qué es un pull request?

*Un pull request es una petición que se hace al propietario de un repositorio original para que este último incorpore los cambios que se sugieren*,*En este ejercicio debermos hacer un pull request sobre el siguiente repositorio:https://github.com/lgarciavelazquez/prueba-pr-iaw_202627*

### Lo que vamos a realizar

*Realizaremos un pull request a este repositorio para solicitar un par de cambios*
### Realización de cosas en mi repositorio local
*En mi repositorio local he creado cosas para yo tenerlas, pero luego meteré todo en el sitio correspondiente,son pasos adicionales los que estoy siguiendo*
* Deberemos cambiar el fichero README.md para añadir un enlace a la lista, donde ponga nuestras iniciales.
* Que vaya al fichero que vamos a crear en el directorio files. A continuación creamos el directorio file y el README que se llama RMCU.
* ![Captura1](images/Creación%20del%20directorio%20files.png)
* Crearemos un fichero en el directorio files, que se llame RMCU.md.
* ![Captura2](images/Creación%20del%20markdown%20RMCU.md.png)
* En el markdown responderemos y a las siguientes preguntas ¿Quienes somos?. ¿Qué asignatura nos gusta más? y ¿Porqué? (debermos utilizar al menos 5 marcas distintas de markdown)
* ![Captura3](images/Archivorcmu.png)
* Versión mejorada
* ![Captura3.3](images/Archivorcmu.version2.0png.png)
* Ahora realizaremos un fork del repositorio prueba-pr-iaw, y nos traemos el repositorio a nuestra cuenta, y por ultimo lo clonamos, y realizamos los cambios especificados en el enunciado.(es decir,tendremos que meter nuestro markdownen files,al repositorio del profesor (prueba iaw), y realizaremos el pull request, para que este acepte los cambios que queremos realizar sobre el repositorio, todo como colaboradores)
* ![Captura4](images/Fork.png)
* ![Captura5](images/repositoriopruebaiaw202627ennuestracuenta.png)
* Para la clonación utilizaremos el siguiente código(y nos llevamos el repositorio para trabajar localmente con el)
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
