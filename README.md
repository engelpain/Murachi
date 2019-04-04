## Script para firmar un PDF con Murachí
Centro Nacional de Desarrollo e Investigación de Tecnologías Libres (CENDITEL) <br>
[CENDITEL](https://www.cenditel.gob.ve/), Mérida - Venezuela<br>
Dirección de Desarrollo<br>
Autor: [Ing. Angelo Osorio](https://twitter.com/Engel_PAIN)<br>
Fecha de Elaboración: 30-01-2019 (dd,mm,aaaa)

### Aspectos técnicos del desarrollo
* OS: Debian 9.8 stretch - 64 Bits
* Navegador: Google Chrome Versión 72.0.3626.109 (Build oficial) (64 bits)
* JavaScript: V8 7.2.502.25

* jQuery v1.11.0
* Forge 0.7.0
* Versión 0.0.12

### Convenciones para el desarrollo del script
Si se quiere escribir un código JavaScript de calidad, con unas características y estructura claras, se debe acostumbrar a seguir una serie de reglas o convenciones.

#### Llamada a los archivos de Javascript
- Por norma general, el código JavaScript debe ser almacenado en su correspondiente fichero de extensión js.
- No se debe embeber dentro del código HTML a menos que sea un proyecto muy pequeño ya que aumenta considerablemente el peso de la página.
- Si se quiere minimizar la demora, la llamada al fichero js, se debe realizar al final del body.

#### Sangrías y tabulaciones
- Se debe usar sangrías para facilitar la lectura del código. Aunque aumenta el tamaño de los ficheros, estos espacios son ignorados y no provocan retrasos en la ejecución. Por norma 

#### Longitud de las líneas
Las líneas no deberían sobrepasar los 80 caracteres. Si hay que seguir la instrucción en la siguiente línea debemos dejar en ésta una sangría de 8 espacios.

#### Comenta tu código
Comentarios útiles y claros teniendo en cuenta que serán leídos posteriormente por nosotros mismos o por otras personas. En general, los comentarios en línea son más claros.

####  Declarar las variables
En JavaScript no es estrictamente necesario declarar las variables antes de usarlas, pero es una buena práctica ya que nos ayudará a evitar errores de variables no declaradas o variables globales mal utilizadas.

####  Declaración correcta de las funciones
No se deben dejar espacios entre el nombre de la función y el primer paréntesis, pero sí después del segundo y antes de la llave. Las instrucciones dentro de la función deben estar tabuladas cuatro espacios y la llave final en línea con la declaración de la función. Estro ayuda a comprender mejor estructuras complejas.
```javascript
function imprimir(valor) {
    alert("valor");
}
```

Si se trata de una función anónima, entonces sí se debe dejar el espacio entre el nombre y el primer paréntesis. Si lo hacemos siempre así será mucho más fácil distinguir entre distintos tipos de funciones.

####  Convenciones de nombres
Los nombres deben estar formados por letras (a .. z, A .. Z) y dígitos (0 .. 9) y guión bajo _. Evitar el uso de caracteres especiales (<*^¨=?) o internacionales ($£àêß).
Las variables deben comenzar con una letra minúscula y las variables globales con mayúscula.
Se deben evitar nombres de una sola letra. Debemos usar nombres descriptivos que ayuden a entender el código. Nunca debemos usar nombres que se puedan confundir con palabras reservadas del lenguaje como break, const, else, new, entre otras.

```javascript
var e = 29; //Mal
var edad = 29; //Bien
```


Usar camelCase para los nombres de objetos, funciones e instancias:
```javascript
var nuevoobjeto = {...} //Mal
var nuevoObjeto = {...} //Bien
function imprimirdatos(){...} //Mal
function imprimirDatos(){...} //Bien
var nuevousuario = new Usuario(); //Mal
var nuevoUsuario = new Usuario(); //Bien
```

- Usar PascalCase (similar a camelCase pero la primera letra en mayúscula) para los nombres de clases y constructores:
```javascript
function moneda(valor){ //Mal
  this.cantidad = valor;
}
function Moneda(valor){ //Bien
 this.cantidad = valor;
}
var nuevaMoneda = new moneda(valor); //Mal
var nuevaMoneda = new Moneda(valor); //Bien
```

- Usar guión  bajo delante de variables o propiedades privadas:
```javascript
this.saldo = 2000; //Mal
this._saldo = 2000; //Bien
```


### Enlaces de interes
- https://medium.com/@davidenq/gu%C3%ADa-de-estilo-convenciones-y-buenas-pr%C3%A1cticas-de-desarrollo-con-javascript-d2e9ef80d63b
- https://tutobasico.com/convenciones-javascript/
- http://snowdream.github.io/javascript-style-guide/javascript-style-guide/es/comments.html
- https://www.aprenderaprogramar.com/index.php?option=com_content&view=article&id=880:javascript-manual-de-estilo-reglas-convenciones-como-crear-objetos-arrays-ejemplos-ejercicio-cu01191e&catid=78&Itemid=206
- http://www.etnassoft.com/2012/10/23/guia-de-estilo-nomenclatura-en-archivos-javascript/
- http://www.solocodigoweb.com/blog/2014/04/30/buenas-practicas-javascript/