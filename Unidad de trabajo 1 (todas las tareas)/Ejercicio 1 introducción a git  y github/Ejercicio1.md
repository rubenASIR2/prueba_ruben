# Unidad de trabajo 1 - Introducción al github
# Ejercicio 1
# Rubén Marcos Cuadrado Ugbomah 
# 2º Administración de sistemas informáticos en red 
# Implantación de aplicaciones web



<!--Vamos a crear un nuevo repositorio llamado prueba2_tu_nombre.-->
## Creación de un repositorio llamado prueba2_ruben_2

#### En primer lugar, nos dirigiremos al github, y nos iremos a la pestaña, para crear nuevos repositorios, a continuación crearemos uno con el nombre correspondiente.

**A continuación adjunto las capturas de pantalla correspondientes**

![Captura1](images/Captura1-Creaciónrepositoriogithub.png)
![Captura2](images/Captura2-Creaciónrepositoriogithub.png)


<!-- En esta ocasión, se creara primero el repositorio local en Windows (usando git init). El repositorio debe contener, al menos, dos archivos de texto: archivo1.txt y archivo2.txt. El contenido de ambos archivos es libre. -->



## Creación del repositorio local en Windows + conexion con un repositorio remoto + creacion archivos y subida de los mismos.
### Seguiremos los siguientes pasos:
* creamos el repositorio local, con el mismo nombre que el remoto (prueba2_ruben)
* mkdir prueba2_ruben (el comando mkdir para crear directorios)
* ![Captura1](images/Creacionrepositorio-mkdirprueba2_ruben.png)
* creamos los ficheros archivo1.txt y archivo2.txt, mediante el comando echo.
* ![Captura1](images/Creacion%20repositorio-Creacion%20de%20los%20ficheros.txt.png)
* git init (iniciaremos el repositorio)
* ![Captura1](images/Creacionrespositorio-inicializar%20el%20repositorio%20git%20init.png)
* git add . (añadiremos archivo1.txt y archivo2.txt)
* ![Captura1](images/Creacionrepositorio-gitadd%20y%20gitstatus.png)
* git commit -m "añadir archivo1 y archivo2"
* ![Captura1](images/Creacionrepositorio-gitcommitarchivos.png)
* git branch -M main (Cambiamos el nombre de la rama a main)
* ![Captura1](images/Creacionrepositorio-cambiodelaramaamain.png)
* git remote add origin  git remote add origin https://USERNAME:TOKEN@github.com//REPO.git  
* ![Captura1](images/Creacionrepositorio-Agregarconexionremota.png)
* git push origin main
* ![Captura1](images/Captura-Creaciónrepositoriogitpushoriginmain.png)
* Comprobación en el repositorio remoto
* ![Captura1](images/Captura-Comprobacionrepositorioremoto.png)

<!-- Clona el repositorio remoto en tu máquina virtual Linux Debian (usando git clone). -->
### A continuación clonaremos el repositorio remoto, en nuestra maquina virtual, Linux Debian, para ello al tendremos en adaptador puente.
### Instalación y configuración de Git en una máquina virtual Debian 12

En primer lugar, se encendio  una máquina virtual con el sistema operativo **Linux Debian 13**. 

Una vez dentro de la máquina virtual, se comprobó si Git estaba instalado. En caso de no estar disponible, se procedió a actualizar los paquetes del sistema mediante el siguiente comando:

```bash
apt update
```
![Captura1](images/Actualizacion%20maquina%20debian.png)
![Captura1](images/Actualizacion%20maquina%20debian2.png)
Posteriormente, se instaló Git utilizando:

```bash
apt install git
```
![Captura1](images/MaquinaDebian-InstalaciónGit.png)
![Captura1](images/Instalacion%20git%20.png)

Una vez finalizada la instalación, se realizó la configuración inicial de Git. Esta configuración es necesaria para identificar al usuario que realiza los cambios en los repositorios, ya que el nombre y el correo electrónico quedan asociados a los commits realizados.

Para establecer el nombre completo del usuario, se utilizó el siguiente comando:

```bash
git config --global user.name "Nombre Completo"(por privacidad no pongo captura)
```


A continuación, se configuró la dirección de correo electrónico mediante:

```bash
git config --global user.email "correo@ejemplo.com" (por privacidad no pongo captura)
```


Se utilizó la opción `--global` para que esta configuración se aplicase de forma general a todos los repositorios utilizados desde la máquina virtual. De esta manera, no es necesario volver a introducir estos datos para cada repositorio.

Después de configurar Git, se procedió a clonar el repositorio remoto en la máquina virtual Debian 12. Para ello, se obtuvo desde GitHub la URL SSH del repositorio y se utilizó el siguiente comando:

 git clone git@github.com:rubenASIR2/prueba2_ruben.git

![Captura1](images/Clonacionrepositorioendebian.png) 
![Captura1](images/Clonamoselrepositorioeneldebian.png)
![Captura1](images/Debianconlosarchivosactuales.png)



### Modificación y actualización del repositorio

1. Una vez clonado el repositorio, se procedió a realizar una modificación desde el sistema operativo Windows.

2. En primer lugar, se modificó uno de los archivos existentes en el repositorio. Además, se creó un tercer archivo de texto llamado archivo3.txt.
![Captura1](images/Creacionarchivo3.txt,%20en%20el%20repositoriowindows.png)

3. Después de realizar los cambios, se añadieron los archivos modificados al área de preparación de Git mediante el comando:

git add .

![Captura1](images/Agregarmoselarchivo3.txt.png)

4. A continuación, se confirmó la modificación mediante un commit. Para ello, se utilizó el siguiente comando:

git commit -m "Modificación de archivo y creación de archivo3.txt"

![Captura1](images/Commitmodificaciondearchivoycreacionarchivo3.txt.png)

5. Una vez confirmado el cambio, se procedió a subir las modificaciones al repositorio remoto mediante:

git push

![Captura1](images/Gitpushoriginmainarchivo3.txt.png)

6. Finalmente, para actualizar la versión local del repositorio en la máquina virtual Linux Debian 12, se ejecutó el siguiente comando:

git pull

![Captura1](images/Gitpull%20y%20obtencion%20del%20archivo3.txt%20en%20la%20maquina%20debian.png)

7. De esta forma, los cambios realizados desde Windows quedaron disponibles también en la máquina virtual Linux Debian 12, manteniendo actualizada la versión local del repositorio.
