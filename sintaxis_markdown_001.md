---
title: "Sintaxis Básica Markdown"
subtitle: "Markdown - RMarkdown"
author: "Renzo Cáceres Rossi"
date: "2022/11/1978"
output:
  html_document:
    code_download: TRUE
    css: "style_markdown_001.css"
---

<!-- Agregar comentarios a nuestro documento Markdown - HTML tags -->

## Encabezados - Títulos

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Título 1
---------

Título 2
========


## Separaciones - Líneas Horizontales

---

***

---

***


## Negrita - Cursiva - Tachado - Subrayado

**Texto formateado como Negrita**

*Texto formatedo como Cursiva*

***Texto formateado como Negrita y Cursiva***

~~Texto tachado~~

<u>Texto subrayado</u>


## Enlaces - Añadir links a nuestro documento Markdown


<http://iiseutec.com/>{target=_blank}

[IISE - UTEC](http://iiseutec.com/){target=_blank}

[http://iiseutec.com/](http://iiseutec.com/ "Ingresa al IISE UTEC"){target=_blank}


## Imágenes - Añadir imágenes a nuestro documento Markdown

<center>

![](logo_r.png)


![](logo_quarto.png)

</center>

## Código - Añadir código de distintos lenguajes de programación


    summary(mtcars)

La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.


```
x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)


```

```Python

import matplotlib.pyplot as plt
 

eje_x = ['Python', 'R', 'Node.js', 'PHP']
 

eje_y = [50,20,35,47]
 

plt.bar(eje_x, eje_y)
 

plt.ylabel('Cantidad de usuarios')
 

plt.xlabel('Lenguajes de programación')
 

plt.title('Usuarios de lenguajes de programación')
 

plt.show()


```


    SELECT id_usuario,usuario_nombre,usuario_apellido FROM usuarios;
    
```sql

USE Northwind;

SELECT * FROM Products;


```

