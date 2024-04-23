# Arrays

- Un array es una sona de almacenamiento contiuno, donde se puede introducir varios valores cada uno de ellos hubicado en una posocion que ocupa en el array.
- También son denominados arreglos o vectores, y cuando son de dos dimensiones son llamados matrices.
- Los arrays nos brindad la capacidad de almacenar una colección de elementos y acceder a ellos de manera individual.
- Cada elemento se indica mediante se posicion en el array, denominada **indice**, y estos indices son siempre secuenciales.
- En Javascrip son almacenamientos flexibles en términos de los diferentes tipos de datos que podemos almacenar en cada posición de array.

## Crear un array
1. Declarando un array con elementos en linea.

```Javascrip
let miArray = [1, 2, 3];
console.log(miArray);
```

2. Declarando un array con la sintaxis **new Array()**

```Javascrip
let miArray = new array(1, 2, 3,);
console.log(miArray);
```
3. Declarando un array especifico utilizando la sintaxis **new Array** y asignando valores despues.

```Javascrip
let miArray = new array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```
4. Declarando un array con elementos de diferentes tipos de datos

```Javascrip
let miArray4 = [1, "dos", true, {nombre: "juan" edad: 30}];
console.log(miArray4);
```