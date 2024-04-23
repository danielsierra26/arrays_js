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
## Accediendo a la informacion de un array

### Propiedad length
- Devuelve la cantidad de elementos del array.

### Operador [pos]
- permite acceder para leer o modificar el elemento pos del array.

### Metodo at(pos)
- Devuelve el elemento de la posicion pos. El parametro admite valores negativos, lo que significa que empiezan a contar por el final del array.

    ```Javascript
     const letters=["A","B","C"];
     console.log(letters.length);
     console.log(letters[2])
     console.log(letters[5])
      ``` 

## Añadir o eliminar elementos
- push(ele1, ele2): añade uno o varios elementos al final del array. Devuelve el tamaño del array.
     ```Javascript
     let miArray = [1,2,3];
     miArray.push(4)// agrega el elemento 4 al final del array
     console.log(miArray);
      ``` 
- pop():devuelve el ultimo elemento del array y lo eleimina.
    ```Javascript
     let miArray = [1,2,3];
     miArray.pop();// elimina el ultimo elemento del array
     console.log(miArray);
      ``` 
- unshift(ele1, ele2): añade uno o varios elementos al inicio devolviendo el tamaño del array despues de añadidos.
    ```Javascript
     let miArray = [1,2,3];
     miArray.unshift(0);// agrega el elemento 0 al inicio de la array
     console.log(miArray);
      ``` 
- shift(): devuelve el primer elemento del array y lo elimina.

     ```Javascript
     let miArray = [1,2,3];
     miArray.shift();// elimina el primer elemento del array.
    console.log(miArray);
      ``` 

- concat(ele1, ele2): concatena dos arrays.
    ```Javascript
     let miArray = [1,2,3];
     let miOtroArray= [4,5]
     let nuevoArray = miArray.concat(miOtroArray);
    console.log(miArray);
    console.log(miOtroArray);
    console.log(nuevoArray);
      ``` 

- split(separador): a partir de una cadena, crea un arry dividiendo dicha cadena en elementos delimitados por separador.
    ```Javascript
     let miString = "Hola, ¿como estas?";
     let miArray= miString.split("");
    console.log(miArray);
    
    ``` 

- join(separador): a partir de un array, crea una cadena separando cada elemento con el separador.

    ```Javascript
     let miArray = "Hola," , "¿como", "estas?";
     let miString= miArray.join("");
    console.log(mistring);

    
    ```  
   
   
## Busqueda de elementos en un array
- includes(elemento):devuelve true o false si el elemento existe o no dentro del array.

- indexOf(elemento): devueleve la posicion de la primera aparicion del elemento. Si no existe devuelve -1.

- lastIndexOf(elemento): devuelve la posicion de la ultima aparicion del elemento. si no existe, devuelve -1.

## Modificar el array o crea fragmento

- slice(inicio, fin): devuelve un array con los elementos desde la posicion inicio hasta la posicion fin, ambos excluidos.

## Ordenar elementos de un array
- reverse(): invierte el orden de los elementos del array.
- sort():ordena el array alfabeticamente.

-sort(criterio): ordena el array con el criterio determinado por la funcion criterio.

## Borra elementos de un array

- Se puede borra el contenido de un elemento de un array poniendo su valor null o asignando una cadena vacia "".

- Para eliminar completamente un elemento del array se utiliza el operador delete.

## Recorrido de un array
1. Recorrer con un bucle clasico, pasando por todos los elementos.

    
    ```Javascript
    var_dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
    for(i=0;i<dias..length;i++)
    {
        console.log(dias[i])
    }
    
    ```  
2.recorrer con whilw, pasando por todos los elementos.
   
    ```Javascript
    var_dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
    for(let index in dias)
    {
        console.log(dias[index])
    }

    ```  


3. Usando la sentencia for..in.
     ```Javascript
    var_dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
    for(let index in dias)
    {
        console.log(dias[index])
    }
    ```  

## Arrays multidimmensionales
    ```Javascript
   const matrix =[
   [1,2,3],
   [4,5,6],
   [7,8,9]
   ];
    ```  
- Recorrer una matrix utilizando bucles anidados.
   ```Javascript
    var_dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
    for(let i=0;i<matriz.length;i++)
    {
        for(let j=0;matriz.length;j++)
        {
            console.log(matriz[i][j])
        }
        
    }

    ```  

# Ejercicios 

1. Dada una lista de numeros separados por coma, calcular la suma, el mayor, el menor y la media de todos.

2. introducir dos cadenas con elementos separados por coma, y con un boton concatenar las dos cadenasy mostrarlas en pantalla.

3. Introducir uno a uno los elementos en un array a través de un boton. Con otro botón se va eliminado el último elemento. Siempre que se pulse alguno de los batanes de debe mostrar el contenido del array.



4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que sola incluya los números pares y mostrarla.
