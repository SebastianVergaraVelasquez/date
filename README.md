Date(): El constructor Date genera un objeto de tipo Date, cuando se llama devuelve una cadena con la fecha y hora actual (en caso de no especificar nada dentro).

```javascript
const today = new Date();
console.log(today)
```

Si se necesita añadir una fecha y hora concreta se hace de la siguiente manera:

```javascript
const birthday = new Date('August 19, 1975 23:15:30');
```

Cada uno de los siguientes métodos devuelve un valor respecto al objeto Date creado. 

```javascript
const anio = today.getFullYear();
const mes = today.getMonth(); //devuelve un valor de 0 a 11
const dia = today.getDate();
const hora = today.getHours();
const minutos = today.getMinutes();
const segundos = today.getSeconds();
const milisegundos = today.getMilliseconds();
const diaSemana = today.getDay(); //Dìa de la semana(domingo =0, Lunes = 1)
console.log(anio);

```

Existen también los métodos set equivalentes para el listado anterior, estos permiten darle valores deseados al objeto Date.

```javascript

const cumpleanios = new Date('June 03, 1998');

event.setFullYear(1997);

console.log(event.getFullYear()); //imprime 1997
```

------

- Se pueden omitir algunos datos al ingresar una fecha en el objeto, como la hora o el día, pero obligatoriamente se debe especificar el año.
