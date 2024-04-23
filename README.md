# Arrays

- Un array es una zona de almacenamiento continuo, donde se pueden introducir variosvalores, cada uno de ellos ubicado por la posición que ocupa el array.
- También son denominados arreglos o vectores, y cuando son de dos simensiones son llamados matrices.
- Los arrays nos brindan la capacidad de almacenar una colección de elementos y acceder a ellos de manera indivudual.
- Cada elemento se identifica mediante su posición en el array denominada **indice**, y estos indices son siempre secuenciales.
- En Javascript son altamente flexibles en términos de los diferentes tipos de datos que podemos allmacenar en cada posición del array.

## Crear un array

1. Declarando un array con elementos en linea

```Javascript
console.log("--------------------");
console.log("Arrays en Javascript");
console.log("--------------------");
console.log("1. Declarando un array con elementos en linea");
let miArray = [1, 2, 3];
console.log(miArray);
```

2. Declarando un arraycon la sintaxis **newArray()**

```Javascript
let miArray = new Array(1, 2, 3);
console.log(miArray);
```
3. Declarando un array con un tamaño específico utilizando la sintaxis new Array y asignando valores después

```Javascript
let miArray = new Array(3);
miArray=[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```

4.  Declarando un array con elementos de diferentes tipos de datos

```Javascript
let miArray4  = [1, "dos", true, {nombre: "Juan", edad: 30}];
console.log(miArray4);
```

## Accediendo a la información de un array
- Devuelve la cantidad de elementos del array.

### Operador [pos]
-Permite acceder para leer o modificar el elemento pos del array.

### Método at(pos)
- Devuelve el elemento de la posición pos. El parámetro admite valores negativos, lo que significa que empieza a contar por el dinal del array.

```Javascript
const letters = ["A", "B", "C"];
console.log(letters.leight);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eliminar elementos
- push(ele1, ele2); añade uno o varios elementos al final del array. Devuelve el tamaño del array.

```Javascript
let miArray = [1, 2, 3];
miArray.push(4); // Agrega el elemento 4 al final del array
console.log(miArray);
```

- pop(): devuelve el ultimo elemento del array y lo elimina
```Javascript
let miArray = [1, 2, 3];
miArray.pop(); // Elimina el último elemento del array
console.log(miArray);
```
- unshift(ele1, ele2): añade uno o varios elementos al inicio, devolviendo el tamaño del array después de añadidos
```Javascript
let miArray = [1, 2, 3];
miArray.unshift(0); // agrega el elemento 0 al inicio del array
console.log(miArray);
```

- shift(): devuelve el primer elemento del array y lo elimina
```Javascript
let miArray = [1, 2, 3];
miArray.shift(0); // elimina el primer elemento del array
console.log(miArray);
```

- concat(ele1, ele2): concatena dos arrays
```Javascript
let miArray = [1, 2, 3];
let miArray = [4, 5];
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(minuevoArray);
```

- split(separador): a partir de una cadena, crear un array dividiendo dicha cadena en elementos delimitador por separador
```Javascript
let miString = "Hola, ¿cómo estás?";
let miArray = miString.split(" ");
console.log(miArray);
```

- join(separador): a partir
```Javascript
let miArray = ["Hola,", "¿cómo", "estás?"];
let miString = miArray.join(" ");
console.log(miString);
```

## Búsqueda de elementos en un array

- incluides(elemento): devuelve true o false si el elemento existe o no dentro del array
- indexOf(elemento): devuelve la posición de la primera aparición del elemento. Si no existe devuelve -1.
- lastIndexOf(elemento): devuelve la posición de la ultima aparición del elemento. Si no existe devuelve -1.

## Modificar el array o crear fragmentos
- slice(inicio, fin): devuelve un array con los elementos de la posición inicio hasta la posición fin, ambos excluidos.

## Ordenar elementos de un array
- reverse(): invierte el orden de los elementos del array
- sort(): ordena el array alfabeticamente
- sort(criterio): ordena el array con el criterio determinado por la función criterio.

## Borrar elementos de un array
- Se puede borrar el contenido de un elemento de un array poniendo su valor a null o asignando una cadena vacía " ".
- Para eliminar completamenteun elemento del array se utiliza el operador delete.

## Recorrido de un array
1. Recorrer con un bucle clásico, pasando por todos los elementos.
```Javascript
var dias = ["Lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
for(i=0;i<dias.lengt;i++)
{
    console.log(dias[i]);
}
```
2. Recorrer con un while, pasando por todos los elementos
```Javascript
var dias = ["Lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
var i = 0
while(i<dias.length)
{
    console.log(dias[i]);
    i++;
}
```
3. Usando la sentencia for..in
```Javascript
var dias = ["Lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
for(let index in dias)
{
    console.log(dias[index]);
}
```

## Arrays multidimensionales
```Javascript
const matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
```
- Recorrer una matriz utilizando bucles anidados
```Javascript
var dias = ["Lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
for(let i=0;i<dias.lengt;i++)
{
    for(let j=0,matriz[i],length; j++)
    {
        console.log(matriz[i][j]);
    }
}
```

# Ejercicios

1. Dada una lista de números separados por coma, calcular la suma, el mayor, el menor y la media de todos.

2. Introducir dos cadenas con elementos separados por coma, y con un botón concatenar las dos cadenas y mostrarlas en pantalla.