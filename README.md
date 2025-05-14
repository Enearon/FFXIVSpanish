# FFXIVSpanish

## Traducción al español de Final Fantasy XIV
En este repositorio se subirán los ficheros de traducción que necesitan ser traducidos y están siendo traducidos. Estos estarán en Inglés.<br/>

## ¿Cómo contribuyo con la traducción?
Se va a habilitar un proyecto web en el cual se podrá contribuir a la traducción manteniendo la estructura original. La web será publicada en este repositorio.<br/>

## ¿Cómo funcionan los códigos HEX que veo en la traducción?
Estos códigos hacen referencia a las funciones. Por ejemplo; Un código que sea <hex:02080DE905FF04> nos indica un condicional, en programación un "IF", un "ELSE", un "SWITCH" o un "CASE" lo que, por ejemplo, podría referirse a si el personaje es hombre o mujer.<br/>
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
El resultado total se calcula de la siguiente manera:<br/>
```Valor en bytes de la primera palabra (4 Bytes) + Valor en bytes de la segunda palabra (5 bytes) + Valor de los condicionales (6 bytes)* + 1 Byte de control dependiendo del tipo de instrucción = 16 Bytes```<br/>
Es muy importante, dependiendo de la instrucción, que antes de traducir se verifique el valor total y se hagan los cálculos, dado que no todas las instrucciones son iguales y pueden usar mas bytes de control, como por ejemplo, algunas usarán 3 bytes en lugar de 1 adicional a la suma total de la instrucción.<br/>
* En este caso, el valor de la instrucción son 6 bytes por ser un IF (2 Bytes) y un ELSE (4 Bytes).<br/>

Para ver los tipos de instrucción podemos acceder a esta página: https://github.com/xivapi/SaintCoinach/blob/master/SaintCoinach/Text/TagType.cs<br/>

Es muy importante entender como funcionan los hex ya que uno mal puesto podría romper todo el fichero de traducción, así que ante la duda, no lo traduzcas y déjalo para cuando el fichero sea revisado.<br/>
AVISO: NO TODOS LOS HEX SON INSTRUCCIONES. Algunos pueden hacer referencia a letras cursivas, negritas, saltos de línea, etc. Iré añadiendo los que pueda a medida que los recopile en la documnetación.<br/>

## Software para la aplicación de la traducción
El repositorio se usa para trabajar en la traducción y todo el software utilizado es exclusivo para testeo interno; Una vez tengamos un avance significativo se publicará el traductor en releases.

## Términos de Uso
⚠️ Este proyecto no tiene fines comerciales ni busca vulnerar la propiedad intelectual de Square Enix. ⚠️<br/>
Es un esfuerzo de fans, hecho por fans y para fans con el fin de mejorar el acceso al contenido del juego para jugadores hispanohablantes.

## Creditos
Aquí se incluirán a todos aquellos que contribuyan en la traducción.
