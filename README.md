# FFXIVSpanish
## Traducción al español de Final Fantasy XIV
En este repositorio se subirán los ficheros de traducción que necesitan ser traducidos. Estos estarán en Chino, pero a medida que pueda iré cambiando la mayoría al inglés oficial del juego usando los ficheros originales para facilitar el proceso de traducción.

## Uso de los ficheros
Estos ficheros son de libre uso, pero no está permitido usarlos con fines lucrativos. Este proyecto será gratuito y llevado a cabo por la comunidad española.

## Como adquirir los ficheros de traducción y empezar a traducir
### Primera opción
Debéis clonar el repositorio descargándolo en vuestro pc haciendo click en el botón verde de nombre `<> Code`<br/>

![image](https://github.com/Enearon/FFXIVSpanish/assets/1865017/a235341d-5986-4355-8597-41bb0649d379)

Existen tres maneras de descargar;
1. Usando Git desde la consola de comandos usamos el comando: `git clone https://github.com/Enearon/FFXIVSpanish.git`
2. Usando Git si tenemos una clave SSH vinculada con el comando: `git clone git@github.com:Enearon/FFXIVSpanish.git`
3. Haciendo click en `Download Zip` (No recomendable)

Aseguraros principalmente de estar en la rama dev mediante el comando `git checkout dev` y aseguraros de que estáis trabajando en dev con el comando `git branch`.<br/>
Trabajando en local lo haréis en la carpeta del repositorio para que los cambios se guarden; Una vez terminéis y queráis enviar los cambios al repositorio debéis usar el comando: `git add ruta/archivo`.<br/>
Para comprobar que el fichero se ha añadido y podéis hacer el commit se usará el comando `git status`.<br/>
Cuando veaís el fichero modificado en verde tocará enviarlo al repositorio mediante el comando `git commit -m "mensaje del commit"` y, una vez procesado, `git push`.<br/>
Si todo ha ido bien el fichero se habrá subido y estará listo para ser revisado y, si cumple los requisitos, unirlo a la rama main.

### Segunda opción
1. Hacemos click en el selector de rama.

![image](https://github.com/Enearon/FFXIVSpanish/assets/1865017/6213077a-2ad2-47af-9ec6-eed1bcfbd314)

2. Seleccionamos la rama dev.
3. Accedemos a la carpeta resources y dentro de ella a la carpeta rawexd donde podremos seleccionar el fichero que queremos modificar. Es importante estar en la rama dev o no podréis modificarlos.

![image](https://github.com/Enearon/FFXIVSpanish/assets/1865017/d218a5b5-c3ca-4630-92a8-b95202b508b2)

4. Hacemos click en el lapiz arriba a la derecha y comenzamos a editar respetando los siguientes pasos.
5. Cuando terminemos guardaremos y haremos el commit que será revisado y, si cumple los requisitos, se unirá a la rama main.

### Software recomendado para traducir
Se recomienda usar el [VSCode](https://code.visualstudio.com/) como editor de los ficheros.<br/>
Si trabajáis directamente en GitHub el editor es bastante parecido al de Code.<br/>
Se debe respetar la estructura y no añadir saltos de línea o textos muy extensos cuando no sea requerido ya que esto haría que fallara.<br/>
No se pueden cambiar los números; Solo el texto en Chino, Inglés o Español.<br/>

![image](https://github.com/Enearon/FFXIVSpanish/assets/1865017/2796723d-d125-4658-8cdc-9b1c72b20324)

## Software para la aplicación de la traducción
Para ejecutar el Software de Traducción solo se debe ejecutar el JAR y seguir las instrucciones (Se añadirán en un futuro cuando la traducción avance).

## Creditos
Programa original creado por [GpointChen](https://github.com/GpointChen/FFXIVChnTextPatch-GP).<br/>
Traducido por Enearon.
