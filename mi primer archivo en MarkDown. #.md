# Unidad 3 #
## Introduccion al lenguaje de programacion R.

**R**, a diferencia de otros programas, surge para realizar análisis estadísticos. Es de código abierto, lo que significa que **cuaquiera puede contribuir a modificar o generar nuevas cosas**. R ha crecido bastante, permitiendo hacer gran cantidad de cosas.

### paquetes

un paquete es una colección de scrips que alguien escribió, documentó y compiló en un sólo archivo `.R.` Existen alrededor de 13 177 paquetes depositados en el repositorio de CRAN.

Una ventaja es que funciona en diferentes plataformas - es portable -. Permite desarrollar **funciones específicas**. Otra es su gran capacidad gráfica para poder hacer **figuras**. Se puede combinar con muchas **herramientas bioinformáticas y sus respectivos formatos**.

**Bioconductor** es un repositorio exclusivo para paquetes bioinformáticos.

 
### MarkDown en R 

Es posible usar el editor de texto en R como un archivo .rmd, el cual puede ser abeirto en un explorador y ser visualizado de manera elegante.

### Cuándo usar RMD o script.R

Un archivo `.RMD` es útil cuando se hace un reporte final de análisis.el *script* podría ser algo más explicativo. ***Un archivo de .RMD no es ejecutable como script de R***.

## Tipo de funciones y objetos básicos en R
en R los comandos son **funciones** que pueden o no recibir **argumentos** -que sirven para que la funcion trabaje correctamente.

### vectores logicos.

Los vectores de tipo lógico presentan valores de tipo booleano de *verdadero* y de *falso* 

### vectores de caracteres

Son caracteres de texto (*`char`* o *`string`*).

### Vectores factor.

los factores son un tipo de vector que puede tomar un numero **limitado** de valores. Se utilizan como **variables categóricas**

las categorías que puede tomar un vector se llaman: **levels**

para crear un factor primero:    

* se crea un vector:

`genero<-c("female", "male");`

* despues se uitliza la funcion `as.factor(c)`donde *`c`* es nuestro vector.

`as.factor(genero)`

* se establecen los lineves para ese vector:

`genero<-as.factor(genero)`

y se estabelcen los niveles para ese factor.

### vectores de enteros contra numericos ###

Los numeros interos *`int`* son 1,2,3,...n.  

`class`es una función en R que indica el tipo de dato que está dentro de nuestros vectores.


