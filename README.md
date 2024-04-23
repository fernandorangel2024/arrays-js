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