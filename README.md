# FFXIVSpanish

## Traducción al español de Final Fantasy XIV
En este repositorio se subirán los ficheros de traducción que necesitan ser traducidos y están siendo traducidos. Estos estarán en Inglés.<br/>

## ¿Cómo contribuyo con la traducción?
Si tu objetivo es traducir contenido simplemente puedes hacerlo a través del repositorio o descargando el fichero en tu pc y mandándolo de vuelta al repositorio a través de git. Ten presente que los cambios no se verán reflejados instantáneamente ya que el fichero debe pasar por el proceso de Pull Request tras verificarse si es válido o realizar las pertinentes correcciones en el mismo antes de unirlo a la rama principal.<br/>

## ¿Cómo funcionan los códigos HEX que veo en la traducción?
Estos códigos hacen referencia a las funciones. Por ejemplo; Un código que sea <hex:02080DE905FF04> nos indica un condicional, en programación un "IF" y un "ELSE" lo que, por ejemplo, podría referirse a si el personaje es hombre o mujer. <br/>
Pero claro ¿Y que significan todos los números y letras adicioinales? Bueno, vamos a desentrañar lo importante del código y un código completo como ejemplo.<br/>

```<hex:020810E905FF05>Hola<hex:FF06>Adios<hex:03>```<br/>
- 02 - Inicia la instrucción, este valor no debe modificarse nunca.<br/>
- 08 - Indica el tipo de instrucción, en este caso nos indica un condicional IF y ELSE.<br/>
- <code style="color : red">**10** - Nos indica el tamaño total de la instrucción. 10 en Hexadecimal es un equivalente a 16 en Decimal.</code><br/>
- E905 - No sabemos muy bien que indica, pero no debe cambiarse.<br/>
- <code style="color : red">**FF05** - Indica el tamaño en bytes del texto. En este caso "Hola" son 4 bytes, pero se añade un byte.</code><br/>
- <code style="color : red">**FF06** - Indica el condicional ELSE y tiene un valor de 5 bytes, pero al igual que antes, se añade un byte.</code><br/>
- 03 - Cierra la instrucción. No debe cambiarse.<br/>

Los valores que nos interesa cambiar durante la traducción están resaltados en negrita. Estos valores son muy importantes o, de lo contrario, la instrucción no funcionará y dará un error de parse y no cargará o el texto no funcionará como debería.<br/>
Para calcular los valores debe hacerse de la siguiente manera:<br/><br/>
Si una instrucción tiene un valor total de 15 bytes a este valor se le debe sumar 1 byte siendo el total de 16 bytes.<br/>
Al igual, si una palabra que añadimos tiene 4 bytes de longitud se debe añadir 1 byte extra, aplica para ambas.<br/>
En el caso de las funciones Switch podemos encontrar múltiples FF05 por cada case que existe. Son algo mas complicados de calcular, pero se calculan de la misma manera que los IF.<br/>

Para ver los tipos de instrución podemos acceder a esta página: https://github.com/ufx/SaintCoinach/blob/master/SaintCoinach/Text/TagType.cs<br/>

Es muy importante entender como funcionanb los hex ya que uno mal puesto podría romper todo el fichero de traducción, así que ante la duda, no lo traduzcas y déjalo para cuando el fichero sea revisado.<br/>

## Software para la aplicación de la traducción
El repositorio se usa para trabajar en la traducción y todo el software utilizado es exclusivo para testeo interno; Una vez tengamos un avance significativo se publicará el traductor en releases.

## Términos de Uso
Todo el contenido en el repositorio es de libre utilización; El código del programa también se muestra y puede ser modificado, mejorado o cambiado a placer por otros usuarios u otras comunidades que deseen hacer su traducción propia. Este proyecto está hecho con software libre y de manera abierta para todos los usuarios, no está permitido el uso del software o el contenido del repositorio con fines lucrativos.

## Creditos
Aquí se incluirán a todos aquellos que contribuyan en la traducción.
