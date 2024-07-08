# 1 Introduccion

### 1.1 ¿Por qué tener convenciones de código?

Las convenciones de código son importantes para los programadores por varias razones:

- El 80% del costo de por vida de una pieza de software se destina al mantenimiento.

- Casi ningún software es mantenido durante toda su vida por el autor original.

- Las convenciones de código mejoran la legibilidad del software, lo que permite a los ingenieros comprender el nuevo código de forma más rápida y completa.

- Si envía su código fuente como un producto, debe asegurarse de que esté bien empaquetado y limpio como cualquier otro producto que crees.


### 1.2 Expresiones de gratitud

Este documento refleja los estándares de codificación del lenguaje Java presentados en Java Language
Especificación, de Sun Microsystems. Las principales contribuciones son de Peter King, Patrick
Naughton, Mike DeMoney, Jonni Kanerva, Kathy Walrath, Scott Hommel y Traducido al Castellano por Alex T.H.
Para preguntas relacionadas con la adaptación, modificación o redistribución de este documento, por favor
lea nuestro aviso de derechos de autor en http://java.sun.com/docs/codeconv/html/Copyright.doc.html.
Los comentarios sobre este documento deben enviarse a nuestro formulario de comentarios en http://java.sun.com/docs/forms/sendusmail.html.

# 2 Nombres de Archivos

Esta sección enumera los sufijos y nombres de archivos más utilizados.

### 2.1 Sufijos de Archivos

JavaSoft utiliza los siguientes sufijos de archivos:

| Tipo de Archivos  | Sufijo |
| ----------- | ----------- |
| Fuente Java      | .java       |
| Codigo de Bytes de Java   | .class        |


### 2.2 Nombres de archivos comunes
 
Los nombres de archivos utilizados con frecuencia incluyen:

| Nombre del Archivo  | Uso |
| ----------- | ----------- |
| GNUmakefile     | El nombre preferido para los archivos MAKE. Usamos **gnumake** para construir nuestro software.       |
| README  | El nombre preferido para el archivo que resume el contenido de un directorio en particular.|

# 3 Organización de archivos

- Un archivo consta de secciones que deben estar separadas por líneas en blanco y un comentario opcional identificando cada sección.
- Los archivos de más de 2000 líneas son engorrosos y deben evitarse.

Para ver un ejemplo de un programa Java formateado correctamente, consulte “Ejemplo de archivo fuente Java” en la página
19.
 
### 3.1 Archivos fuentes de Java

Cada archivo fuente de Java contiene una única clase o interfaz pública. 
Cuando las clases privadas y las interfaces están asociadas con una clase pública, puede colocarlas en el mismo archivo fuente que la clase pública.
La clase pública debe ser la primera clase o interfaz del archivo.

Los archivos fuente de Java tienen el siguiente orden:

- Comentarios iniciales (consulte “Comentarios iniciales” en la página 4)
- Declaraciones de paquetes e importaciónes; Por ejemplo:
```java
import java.applet.Applet;
import java.awt.*;
import java.net.*;
```
- Declaraciones de clase e interfaz (consulte “Declaraciones de clase e interfaz” en la página 4) 


#### 3.1.1 Comentarios iniciales

Todos los archivos fuente deben comenzar con un comentario estilo C que enumere los programadores, la fecha, un
aviso de derechos de autor, y también una breve descripción del propósito del programa. Por ejemplo:

```java
/*
 * Classname
 *
 * Version info
 *
 * Copyright notice
 */
```
#### 3.1.2 Declaraciones de paquetes e importaciónes

La primera línea que no es de comentario de la mayoría de los archivos fuente de Java es una declaración de **paquete**. Después,
Pueden seguir declaraciones de **importación**. Por ejemplo:
 
```java
package java.awt;
import java.awt.peer.CanvasPeer;
```



