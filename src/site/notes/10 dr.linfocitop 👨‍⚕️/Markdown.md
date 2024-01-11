---
{"dg-publish":true,"permalink":"/10-dr-linfocitop/markdown/","noteIcon":""}
---

#obsidian 
+ Markdown es un *lenguaje* de marcado ligero que se utiliza principalmente *para formatear texto de una manera sencilla y fácil de leer*. Se diseñó originalmente para ser utilizado en la web y se ha convertido en un estándar ampliamente utilizado para la escritura en línea, especialmente en plataformas como *GitHub*, *Reddit* y *Stack Overflow*.
+ No usa etiquetas HTML complicadas. 
+ A continuación, te mostraré algunos ejemplos de cómo puedes utilizar Markdown para formatear texto:
## Formatos de texto
1. *Encabezados*: Puedes crear encabezados utilizando uno o varios signos de almohadilla (#) al comienzo de la línea. Por ejemplo:
```Markdown
# Encabezado de nivel 1
## Encabezado de nivel 2
### Encabezado de nivel 3
```
2. *Enfatizar el texto*: Puedes utilizar asteriscos `(*)` o guiones bajos `(_)` alrededor de una palabra o frase para enfatizarla. Por ejemplo:
```Markdown
*Texto en cursiva* 
_Texto en cursiva_
**Texto en negrita**
__Texto en negrita__
```
3.  *Listas*: Puedes crear listas ordenadas y no ordenadas utilizando guiones (-), asteriscos ``(*)`` o números seguidos de un punto (.). Por ejemplo:
```Markdown
- Elemento 1
- Elemento 2 
- Elemento 3  

1. Elemento 1 
2. Elemento 2 
3. Elemento 3
```
4. *Listas anidadas*: Puedes anidar listas dentro de otras listas utilizando sangría con espacios o tabulaciones. Por ejemplo:
```
- Elemento 1    
	- Subelemento 1.1    
	- Subelemento 1.2 
- Elemento 2    
	- Subelemento 2.1       
		- Subelemento 2.1.1
```
5.  *Enlaces externos*: Puedes crear enlaces utilizando corchetes ([]) para el texto del enlace y paréntesis (()) para la URL. Por ejemplo:
```-Markdown
- [Enlace a Google](https://www.google.com)
```
- [Enlace a Google](https://www.google.com)
6. *Enlaces internos*: Se realizan a otras entradas. Pueden crearse si no existen aún.
```-Markdown
- [[Obsidian]]
```
8.  *Imágenes*: Puedes incrustar imágenes utilizando un signo de exclamación (!), corchetes ([]) para el texto alternativo de la imagen y paréntesis (()) para la URL de la imagen. Por ejemplo:

``` 
![Texto alternativo](https://www.example.com/imagen.jpg)
```
6. *Citas*: Puedes crear citas utilizando el signo mayor que (>). Por ejemplo:
```Markdown
> Esto es una cita
```
> Esto es una cita

1. *Bloques de código*: Puedes resaltar bloques de código utilizando comillas invertidas ``(```)`` al principio y al final del bloque. También puedes especificar el lenguaje de programación para obtener resaltado de sintaxis. Por ejemplo:
````
```Python
def saludar():
	print("¡Hola, mundo!")
saludar()
```
````

```Python
def saludar():
	print("¡Hola, mundo!")
saludar()
```
8. *Líneas horizontales*: Puedes crear líneas horizontales utilizando tres guiones (``-``), asteriscos ``(*)`` o guiones bajos ``(_)``. Por ejemplo:
``` yaml
---
***
___
```
---
___
***

9. *Tachado de texto*: Puedes tachar texto utilizando dos virgulillas (~) alrededor de la palabra o frase. Por ejemplo:
``` markdown
~~Texto tachado~~
```
~~Texto tachado~~

10. *Tablas*: Puedes crear tablas utilizando barras verticales (|) para separar las columnas y guiones (-) para separar la cabecera de la tabla. Por ejemplo:
``` css
| Nombre  | Edad | 
|---------|------| 
| Juan    | 25   | 
| María   | 30   |
```
| Nombre  | Edad | 
|---------|------| 
| Juan    | 25   | 
| María   | 30   |


12. Resaltado de código: Puedes resaltar código dentro de una línea utilizando comillas invertidas `(``)` `. Por ejemplo:
```
El comando `print()` muestra un mensaje en la consola.
```


17.  Notas al pie de página: Puedes agregar notas al pie de página utilizando corchetes ([]) y paréntesis (()) para el texto de la nota y la referencia. Por ejemplo:
`Esto es un ejemplo de una nota al pie de página[^1].  [^1]: Esta es la explicación de la nota al pie de página.`


`<span style="color: blue;">Este texto está resaltado en azul.</span>`



`H<sub>2</sub>O es la fórmula del agua. x<sup>2</sup> representa x al cuadrado.`

`[![Texto alternativo](http://img.youtube.com/vi/VIDEO_ID/0.jpg)](http://www.youtube.com/watch?v=VIDEO_ID)`


`[Texto de enlace de audio](ruta/al/archivo.mp3)`

`def saludar():     print("¡Hola, mundo!")  saludar()`



`Esto es un texto de ejemplo.^1^ 
{ #1}
^ Esto es una nota al margen relacionada con el texto anterior.`


`<span style="font-size: 20px;">Este texto tiene un tamaño de fuente de 20 píxeles.</span>`



`![Texto alternativo](ruta/a/la/imagen.jpg){width=400 height=300}`

