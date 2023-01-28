## Variables y operaciones

1. Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una variable y para qué sirve? Una variable es la representación de un lugar que reservamos en memoria para guardar un valor.El valor puede ser cualquier tipo de dato, inclusive objetos o funciones.

- ¿Cuál es la diferencia entre declarar e inicializar una variable? declarar una variable es asignarle un valor a la misma, mientras que inicializarla es utilizarla.

- ¿Cuál es la diferencia entre sumar números y concatenar strings? sumar es una operacion matematica, ejemplo: 1+1 = 2, mientras que concatenar un strig es unir los valores de los string "Hola " + "soy Guido" nos daria "Hola soy Guido"

- ¿Cuál operador me permite sumar o concatenar? el operador +

2. Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre = string
- Apellido = string
- Nombre de usuario de Platzi = string
- Edad = number
- Correo electrónico = string
- Mayor de edad = boolean
- Dinero ahorrado = number
- Deudas = number

3. Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

```
let Nombre = "Guido";
let Apellido = "Garcia";
let NombreDeUsuarioDePlatzi = "Guido";
let Edad = 34;
let CorreoElectronico = "guido2288@gmail.com";
let MayorDeEdad = true;
let DineroAhorrado = 190000;
let Deudas = 1500;
```

4. Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

```
let nombreCompleto = `${Nombre} ${Apellido}`;
let dineroReal = DineroAhorrado - Deudas;

```

## Funciones

1. Responde las siguientes preguntas:

- ¿Qué es una función? un conjunto de instrucciones que realizan una tarea. Tienen una entrada y siempre retornan un valor.

- ¿Cuándo me sirve usar una función en mi código? Cuando necesitamos realizar una operacion, que modifique un valor.

- ¿Cuál es la diferencia entre parámetros y argumentos de una función? Los parámetros son las variables declaras y solicitadas en nuestra función, al momento de realizar el llamado de nuestra funciones nos exigirá declarar nuestras variables que vendrían a ser nuestros argumentos de la funció

2. Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```
const proceso = (completeName, nickname) => {
  return console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
}

```

## Condicionales

1. Responde las siguientes preguntas:

- ¿Qué es un condicional? lineas de codigo que permiten controlar que procesos se van a ejecutar, si se cumplen o no ciertas condiciones.

- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias? if , else , switch

- ¿Puedo combinar funciones y condicionales? Si se puede

2. Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

```
const tipoDeSuscripcion = "Free";

const evaluarSuscripcion = (suscripcion) => {
  if (suscripcion === "Free") {
    return console.log("Solo puedes tomar los cursos gratis")
  } else if (suscripcion === "Basic") {
    return console.log("Puedes tomar casi todos los cursos de Platzi durante un mes")
  } else if (suscripcion === "Expert") {
    return console.log("Puedes tomar casi todos los cursos de Platzi durante un año")
  } else if (suscripcion === "ExpertPlus") {
    return console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año")
  } else {
    return console.log("Error en datos ingresados")
  }
}

evaluarSuscripcion(tipoDeSuscripcion)

```

3. Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

```
const tipoDeSuscripcion = "Free";

const evaluarSuscripcion = (suscripcion) => {
  if (suscripcion === "Free") {
    return console.log("Solo puedes tomar los cursos gratis")
  } if (suscripcion === "Basic") {
    return console.log("Puedes tomar casi todos los cursos de Platzi durante un mes")
  } if (suscripcion === "Expert") {
    return console.log("Puedes tomar casi todos los cursos de Platzi durante un año")
  } if (suscripcion === "ExpertPlus") {
    return console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año")
  }
  return console.log("Error en datos ingresados")

}

evaluarSuscripcion(tipoDeSuscripcion)

```

## Ciclos

1. Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo? Un bucle (loop) o ciclo repetitivo es una estructura de control que te permite realizar una o varias instrucciones mientras una condición sea verdadera.

- ¿Qué tipos de ciclos existen en JavaScript? For - While - Foreach - Do While

- ¿Qué es un ciclo infinito y por qué es un problema? Cuando en un ciclo la condición siempre es verdadera se genera un ciclo infinito, pues nunca saldrá del ciclo y el programa no termina.

-¿Puedo mezclar ciclos y condicionales? si se puede, generar ciclos que se ejecutan si se cumple cierta condicion.

2.  Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```
let i = 0;
while (i < 5) {
   console.log("El valor de i es: " + i);
   i++
 }
```

```
let i = 10;
while (i >= 2) {
  console.log("El valor de i es: " + i);
  i--
}
```

3. Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

```
let num = 10;
let num2 = 10;
const result = num + num2;
let questions = {
  q1: `Cuanto es ${num} + ${num2}`
}
function Quizzer() {
  let userInput = prompt(questions.q1);
  if (userInput == result) {
    alert("Felicitaciones, respondiste correctamente el desafio");
  } else {
    alert("lamentablemente, tu respuesta es incorrecta, sigue practicando!");
  }
}
Quizzer();
```

## Listas

1. Responde las siguientes preguntas:

- ¿Qué es un array? Un array es una estructura de datos que permite almacenar una serie de datos localizados por índices y separados por comas.

- ¿Qué es un objeto? Un objeto es una estructura de datos que permite almacenar valores mediante propiedad - valor a través de la sintaxis de llaves ({}) y separados por comas.

- ¿Cuándo es mejor usar objetos o arrays? Los arrays se usan para series que poseen valores simples, mientras que los objetos son utilizadas para las series en que hay distintos objetos y propiedades con diferentes valores.

- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays? Si se puede incluir objetos como un elemento de un array

2. Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento

```
const primerElemento = (array) => {
  return console.log(array[0]);
};

primerElemento([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
```

3. Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

```
const contador = (array) => {

  let i = 0

  while (array[i] <= array.length) {
    console.log(array[i])
    i++
  }

};

contador([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
```

4. Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

```
let auto = {
  marca: "Toyota",
  color: "Negro",
  annio: 2010
};

const elementosObjeto = (objeto) => {

  for (let i = 0; i < Object.values(objeto).length; i++) {
    console.log(Object.values(objeto)[i])
  }

};

elementosObjeto(auto);

```
