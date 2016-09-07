# leccion-20-e2

###Código inicial

``` javascript

1. var feature = "closures";
2. (function () {
3.	if ( typeof feature === "undefined"){         
4.		var feature = "callbacks";         
5.		console.log("JS coders love its " + feature );     
6.	} else {       
7.		console.log("JS developers love its " + feature );     
8.	}
9. })();
```

###Código final

``` javascript

1.(function () {
2.	var feature = "closures";
3.	if ( typeof feature === "undefined"){         
4.		var feature = "callbacks";         
5.		console.log("JS coders love its " + feature );     
6.	} else {       
7.		console.log("JS developers love its " + feature );     
8.	}
9. })();
```
###Solución

En la línea 1 del código inicial está definida la variable feature = "clousure" , pero al colocarla ahí, de manera global, la función anónima autoejecutable no la está usando ya que para esa función anónima autoejecutable la variable no está definida y por eso muestra el primer mensaje, pero al colocarla en la línea 2, dentro de la función anónima, la variable ya estaría definida de manera local y ya no sería verdad la primera condición, sino la segunda y muestra el segundo mensaje.
