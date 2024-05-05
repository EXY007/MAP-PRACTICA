```javascript
const numeros = [1,2,3,4,5];

const multiplicados = numeros.map(x => x*2)
console.log(multiplicados)
console.log("fun")

const pares = numeros.map(x => [x,x])
console.log(pares)


//FUNCION SUMAR
function suma(numerosArray)  {
 var result = 0;
 for (let i = 0; i < numerosArray.length; i++) {

    result = result + numerosArray[i] 
 }
return result;

}
console.log(suma(numeros))//aplico la funcion a numeros(es un array)

const mascotas =[
    { nombre: 'Puchini', edad: 12, tipo: 'perro' } ,
    { nombre: 'Chanchito feliz', edad: 3, tipo: 'perro'},
    { nombre: 'Pulga', edad: 10, tipo: 'perro'},
    { nombre:'Pelusa', edad: 12, tipo: 'gato'}
    ]

//x representa cada elemento del arreglo //.MAP DEVUELVE OTRO ARREGLO
const edades = mascotas.map(x => x.edad)  
console.log(edades)// imprime un nuevo arreglo solo con las edades
console.log(suma(edades))//aplico ese arreglo a la funcion sumar
console.log("========")
let sumaEdades = (suma(edades))//aplico ese arreglo a la funcion sumar en variable separad
console.log(sumaEdades/edades.length)//imprimo el promedio de las edades
```