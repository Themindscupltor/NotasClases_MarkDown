#Programacion con R y paquetes bioinformáticos
*22 de enero, 2019*
     
##R studio.
**vectores**

factores: es un vector con categorías limitadas

```
x <- c("Female", "male", "Female").   
x <- as.factors(x)
levels(x)
```
El output será:

```
[1] "Female" "Male"   "Female"

```

## listas ##

agrupa vectores y los pone independientemente

ej:


```
x<-list(1:3, letters[1:3], is.numeric)
```

el output será:

```
[[1]]
[1] 1 2 3

[[2]]
[1] "a" "b" "c"

[[3]]
function (x)  .Primitive("is.numeric")

```

## Matrices

Todos los valores deben tener el mismo tipo:   

* numoeros
* caracteres
* valores logicos

etc.

 La función en R para generar la matriz es 
 
 ```
 x<-matrix (1:12, nrow=4, ncol=3)
 ```
 funciones útiles para matrices:
 
```
rownames(x)<-xc("a", "b", "c", "d")    # nombre de las filas
colnames(x)<-x("1","2","3","4")         #nombre de las columnas
dim(x)                              	# dimensiones de la matrix 
nrow(x)									#numero de filas
ncol(x)									#numero de columnas
```

##Data Frames

Muchas veces, nuestros datos en una matriz pueden presentarse diferentes tipos de datos, como caracteres, numeros, valores lógicos, etc.

Los **Data Frames** son matrices en donde pueden existir diferentes tipos de caracteres.   

```
DataFrames

x<-data.frame(sp=c("sp1", "sp2", "sp3", "sp4"),
        sexo=c("Female", "Male","Female", "Male"), 
        edad=c(20, 30, 40, 10))

x
```
**Cómo agregar una columna nueva**  

``` 
pop<-c("Australia", "japón", "Antillas","Mexico").  

nuevax<-cbind(x,pop).  

```  

**mostrar las primeras dos filas de nuevas**

```
nuevax[c(1:2),]
```

## Resumen de R

Podemos tener en R:

* expresiones matemáticas
* Strings de texto
* Valores Lógicos
* funciones
* variables

##Paquetes

Los paquetes en R son funciones particulares que desempeñan una funcion específica. 

cada vez que queramos usar un paquete, hay que usar la funcion `library()`

**¿cómo citar R?**

A través de la funcion `citation(paquete_específico/base)`es posible obtener la cita necesaria del paquete que estamos usando.

##Cargar archivos en R

se lleva a cabo con funciones específicas de tipo `read`

## loops

**For**

#ejercicios unidad 3

###crea una variable con el logaritmo base 10 de 50 y súmalo a otra variable cuyo valor sea igual a 5.


### suma el número 2 a todos los números entre 1 y 150.

###¿cuántos números son mayores a 20 en el vector -13432:234?

###Carga en R el archivo Prac_Uni3/maices/meta/maizteocintle_SNP50k_meta_extended.txt y ponlo en un objeto de R llamado meta_maiz.


###Escribe un for loop para que divida 35 entre 1:10 e imprima el resultado en la consola.

###Modifica el loop anterior para que haga las divisiones solo para los números nones (con un comando, NO con c(1,3,...)). Pista: next.

###Modifica el loop anterior para que los resultados de correr todo el loop se guarden en una df de dos columnas, la primera debe tener el texto "resultado para x" (donde x es cada uno de los elementos del loop) y la segunda el resultado correspondiente a cada elemento del loop. Pista: el primer paso es crear un vector fuera del loop. Ejemplo:

```
elefantes<-character(0)
for (i in 2:10){
  elefantes<-rbind(elefantes, (paste(i, "elefantes se columpiaban sobre la tela de una araña")))
}
elefantes
```


###Abre en RStudio el script Prac_Uni3/mantel/bin/1.IBR_testing.r. Este script realiza un análisis de aislamiento por resistencia con Fst calculadas con ddRAD en Berberis alpina.Lee el código del script y determina:

* ¿qué hacen los dos for loops del script?
* ¿qué paquetes necesitas para correr el script?
* ¿qué archivos necesitas para correr el script?