<span class="bigTitle">JavaScript For Cats</span>
## Una introducción para nuevos programadores.<span class="right">![cat](images/substack-cats.png)</span>
### *¡Tan fácil que tu compañero humano podría hacerlo también!*

JavaScript es un lenguaje de programación o, en otras palabras, un medio por el cual una computadora recibe instrucciones de hacer cosas. Al igual que uno controla a los humanos con silbidos y maullidos, uno controla las computadoras con declaraciones escritas en un lenguaje de programación. ¡Todos los navegadores web entienden JavaScript y usted puede aprovechar eso para hacer que las páginas web hagan locuras!

JavaScript comenzó como una forma de hacer que las páginas web sean más interactivas. Hoy en día, JavaScript se ejecuta en más lugares que solo navegadores web: ¡se ejecuta en servidores web, teléfonos e incluso robots! Esta página le enseñará algunos conceptos básicos de JavaScript para que pueda comenzar a trabajar en poco tiempo *.


\* *Actual time: más que ninguno. Probablemente una o dos horas. Además, como eres un gato, es menos probable que corras y más probable que te tumbes al sol*

JavaScript for Cats is [CC0 Licensed](https://creativecommons.org/publicdomain/zero/1.0/)

## Tabla de Contenidos

- [La consola](#basics)
- [Strings](#strings)
- [Values and variables](#values)
- [Usando functions](#functions)
- [Built(consutruido) in JS functions](#standard-library)
- [Download new JS functions](#third-party-javascript)
- [Escribir new functions](#writing-functions)
- [Loops](#loops)
- [Arrays](#arrays)
- [Objects](#objects)
- [Callbacks](#callbacks)
- [Recommended reading](#recommended-reading)

## No seas un gato asustado

<span class="right">![cat](images/yarnify.png)</span>

Siempre aterrizarás de pie, ¡incluso cuando programes! A diferencia de [manipular un vaso de agua](images/dealwithit.gif) en su computadora portátil, nada en estos tutoriales dañará su computadora de ninguna manera, incluso si escribe mal un comando o hace clic en el botón incorrecto. Al igual que los gatos, los programadores informáticos cometen errores todo el tiempo: escribir mal las cosas, olvidar citas o corchetes y olvidar cómo funcionan las funciones básicas (y el hilo, el láser). Los programadores se preocupan más por hacer que funcione _eventualmente_ en lugar de tratar de hacerlo funcionar la primera vez. ¡La mejor manera de aprender es cometiendo errores!

¡Así que no seas un gato asustado! Lo peor que puede pasar es que quizás tengas que actualizar esta página en tu navegador web si te quedas atascado. Sin embargo, no se preocupe, esto sucederá muy raramente.

## <a id="basics" href="#basics">#</a> Lo básico

Hay JavaScript ejecutándose en esta página en este momento. Juguemos un poco con eso. En aras de la simplicidad, supondré que está utilizando Google Chrome para leer esta página (si no lo es, probablemente sea más fácil para ambos si sigue con Chrome).

Primero, haga clic derecho en cualquier lugar de la pantalla y presione **Inspeccionar elemento** , luego haga clic en la pestaña **Consola** . Deberías ver una cosita que se ve así:

![console](images/console.gif)

Esta es una consola, también conocida como "línea de comando" o "terminal". Básicamente es una forma de escribir una cosa a la vez en una computadora e inmediatamente obtener la respuesta de las computadoras. Son súper útiles como herramienta de aprendizaje (todavía uso la consola casi todos los días que estoy codificando).

La consola hace algunas cosas geniales. ¡Aquí comencé a escribir algo y la consola me está ayudando dándome una lista de todas las cosas posibles que podría seguir escribiendo! Otra cosa que puedes hacer es escribir 1 + 1en la consola y luego presionar la Entertecla y ver qué sucede.

Usar la consola es una parte muy importante del aprendizaje de JavaScript. Si no sabe si algo funciona o cuál es el comando para algo, ¡vaya a la consola y descúbralo! Aquí hay un ejemplo:

### <a id="strings" href="#strings">#</a> Strings

Como soy un gato, quiero reemplazar cada instancia de la palabra `dog` en Internet `those blasted dogs`. Primero vaya a su consola y escriba algunas oraciones que contengan la palabra`dog`l menos una vez. En JavaScript, un grupo de letras, números, palabras o cualquier otra cosa se conoce como un **String** (como en una cadena de caracteres). Las cadenas tienen que comenzar Y terminar con una comilla. Simple`'` o doble `"` está bien, solo asegúrate de usar lo mismo al principio que al final.

![console](images/console-strings.gif)

¿Ves el desagradable mensaje de error? No se preocupe, no violó ninguna ley. SyntaxError ILLEGAL es la forma en que suena cuando los robots le dicen que su programa tiene un problema. Las primeras dos oraciones tenían comillas coincidentes al principio y al final, pero cuando mezclé comillas simples y dobles, me asusté.

OK, para arreglar una de estas oraciones (al reemplazar dogcon nuestra versión mejorada) primero tenemos que guardar la oración original para que podamos recuperarla más tarde cuando hagamos nuestra magia de reemplazo. ¿Te das cuenta de cómo la cadena se repite en rojo cuando la escribimos en la consola? Esto se debe a que no le hemos dicho que guarde la oración en ningún lugar, por lo que solo la devuelve de inmediato (o nos devuelve un error si desordenamos algo).

### <a id="values" href="#values">#</a> Values y variables

**Los Valores** ason los componentes más simples en JavaScript. `1` es un valor, `true` es un valor, `"hello"` es un valor, `function() {}`es un valor, ¡la lista continúa! Hay un puñado de diferentes **tipos** de valores en JavaScript, pero no es necesario que los revisemos de inmediato, ¡los aprenderá de forma natural cuanto más codifique!

Para almacenar valores usamos cosas llamadas **variables** . La palabra 'variable' significa 'puede cambiar' y se usa porque las variables pueden almacenar muchos tipos diferentes de valores y pueden cambiar su valor muchas veces. Son más o menos como buzones. Ponemos algo en una variable, como nuestra oración, y luego le damos a la variable una dirección que podemos usar para buscar la oración más tarde. En la vida real, los buzones tienen que tener números de apartado de correos, pero en JavaScript generalmente solo se usan letras minúsculas o números sin espacios.



![console](images/console-variables.gif)

`var`es la abreviatura de variable y los  `=` edios almacenan la cosa en el lado derecho en la cosa en el lado izquierdo . Además, como puede ver, ahora que estamos almacenando nuestra oración en una variable, la consola no solo devuelve nuestra oración de inmediato, sino que nos da el `undefined` que significa que *no había nada que devolver* .

Si simplemente escribe un nombre de variable en la consola, imprimirá el valor almacenado en esa variable. Una nota sobre las variables es que, de forma predeterminada, desaparecen cuando cambia a una página diferente. Si`dogSentence` tuviera que presionar el botón Actualizar en Chrome, por ejemplo, mi variable se borraría y sería como si nunca hubiera existido. Pero no se preocupe demasiado por esto por ahora: puede presionar las flechas hacia arriba o hacia abajo en su teclado mientras está en la consola para revisar todo lo que ha ingresado recientemente.

### <a id="functions" href="#functions">#</a> Functions

Ahora que tenemos nuestra oración almacenada en una variable, ¡cambiemos una palabra almacenada en ella! Podemos hacer esto realizando una *function*. Las *Functions* son un tipo de valor que, bueno, cumple una *función* específica (propósito o acción de AKA) para nosotros. Llamarlos "acciones" sonaba extraño, supongo que en su lugar usaron la palabra "functión".

¡JavaScript tiene una función llamada `replace` que hace exactamente lo que queremos! Las funciones toman cualquier número de valores entre paréntesis (cero, uno o muchos) y devuelven nada (`undefined`) o la cadena modificada. El `replace` function está disponible para usar en cualquier cadena y toma dos valores: los caracteres que se deben extraer y los caracteres que se deben intercambiar. Se vuelve confuso describir estas cosas, así que aquí hay un ejemplo visual:

![console](images/console-replace.gif)

¿Te das cuenta de que el valor de`dogSentence` es el mismo incluso después de ejecutarlo `replace` ? Esto se debe a que la `replace` function, (y la mayoría de las funciones de JavaScript) toma el valor que le damos y devuelve un **nuevo valor** , sin modificar el valor que pasamos. Dado que no almacenamos el resultado (no hay ningún`=` a la izquierda lado de la función de reemplazo) acaba de imprimir el valor de retorno en nuestra consola.

### <a id="standard-library" href="#standard-library">#</a> The "standard library"

Tal vez se pregunte qué otras funciones están disponibles en JavaScript. La respuesta: una tonelada. Hay muchas bibliotecas estándar incorporadas de las que puede aprender en MDN (un sitio administrado por Mozilla que tiene mucha información ingeniosa sobre tecnologías web). Por ejemplo, [aquí está la página MDN en el objeto Math de JavaScript](https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Global_Objects/Math).

### <a id="third-party-javascript" href="#third-party-javascript">#</a> Third-party JavaScript (JavaScript de terceros)

También hay una gran cantidad de código JavaScript disponible que **no** está **integrado**. JavaScript de terceros generalmente se conoce como "biblioteca" o "complemento". Uno de mis favoritos se llama **Underscore.js**. ¡Vamos a agarrarlo y cargarlo en nuestra página! Primero vaya al sitio de Underscore, [http://underscorejs.org/](http://underscorejs.org/), haga clic en el enlace de descarga (generalmente uso versiones de desarrollo porque son más fáciles de leer pero ambas le darán la misma funcionalidad básica), y luego copie todo el código en su portapapeles (puede usar Seleccionar todo en el menú Editar para seleccionar todo). Luego péguelo en su consola y presione enter. Ahora su navegador tiene una nueva variable:`_`. El subrayado te ofrece un montón de funciones útiles para jugar. Aprenderemos más sobre cómo usarlos más adelante.

![console](images/underscore.gif)

### <a id="writing-functions" href="#writing-functions">#</a> Making new functions

No está limitado a usar las funciones de otras personas, también puede escribirlas usted mismo. ¡Es muy fácil! Hagamos una función llamada `makeMoreExciting` que agregue un montón de signos de exclamación al final de una cadena.

    function makeMoreExciting(string) {
      return string + '!!!!'
    }

En mi cabeza lo leí en voz alta así: "hay una función llamada 'hacer más emocionante' que toma una cadena y devuelve una nueva copia de esa cadena que tiene un montón de signos de exclamación al final". Así es como escribiríamos esto en la consola manualmente si no estuviéramos usando una función:

![console](images/custom-function-manually.gif)

La expresión `string + '!!!!'` devuelve una nueva cadena y nuestra variable llamada `string` permanece igual que antes (ya que nunca la actualizamos a otra cosa con `=`).

Usemos nuestra función en lugar de hacerlo manualmente. Primero, pegue la función en la consola y luego **invoque** la función **pasando** una cadena:

![console](images/custom-function-call.gif)

También puede llamar a la misma función pasando una variable que apunta a una cadena (en el ejemplo anterior, simplemente escribimos la cadena directamente como un valor en lugar de guardarla primero en una variable):


![console](images/custom-function-call-variable.gif)

The line `makeMoreExciting(sentence)` is equivalent to saying `sentence + '!!!!'`. What if we wanted to **modify in-place** (aka update) the value of sentence? Simply save the return value of the function back into our `sentence` variable:

    var sentence = "time for a nap"
    sentence = makeMoreExciting(sentence)

¡Ahora `sentence` tendrá los signos de exclamación! Tenga en cuenta que solo tiene que usarlo `var`cuando está **inicializando** una variable, la primera vez que la usa. Después de eso, no debe usar a `var`menos que desee reiniciar (restablecer / borrar / vaciar) la variable.

¿Qué pasaría si sacamos la `return` declaración en nuestra función?

![console](images/custom-function-no-return.gif)

¿Por qué está `sentence`vacío? ¡Porque las funciones regresan `undefined`por defecto! Puede elegir devolver un valor `return`e ing algo. Las funciones deben tomar un valor y, si cambian el valor o crean un nuevo valor que se supone que se usará más adelante, `return`un valor (hecho divertido: un término elegante para este estilo es _programación funcional_ ). Aquí hay otra función que no devuelve nada, sino que utiliza un método diferente para mostrarnos el resultado:

```js
function yellIt(string) {
  string = string.toUpperCase()
  string = makeMoreExciting(string)
  console.log(string)
}
```

Esta función, `yellIt` utiliza nuestra función anterior `makeMoreExciting`, así como el método String incorporado en[toUpperCase](https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Global_Objects/String/toUpperCase).Los Methods son solo un nombre para una función cuando pertenece a algo, en este caso `toUpperCasees` una función a la que pertenece, por `String` lo que podemos referirnos a ella como un método o una función. `makeMoreExcitingpor` otro lado, no pertenece a nadie, por lo que sería técnicamente incorrecto referirse a él como un método (confuso, lo sé).

La última línea de la función es otra función incorporada que simplemente toma los valores que le da y los imprime en la consola.

![console](images/custom-function-console-log.gif)

Entonces, ¿hay algo mal con la `yellIt` functión anterior ? ¡Depende! Estos son los dos tipos principales de funciones:

funciones que modifican o crean valores y los devuelven
las funciones toman valores y realizan alguna acción que no se puede devolver

`console.log` es un ejemplo del segundo tipo de función: imprime cosas en su consola, una acción que puede ver con los ojos pero que no puede representarse como un valor de JavaScript. Mi propia regla general es tratar de mantener los dos tipos de funciones separadas entre sí, así que así es como reescribiría la `yellIt` functión:
```js
function yellIt(string) {
  string = string.toUpperCase()
  return makeMoreExciting(string)
}

console.log(yellIt("i fear no human"))
```

De esta manera, se `yellIt` vuelve más **genérico** , lo que significa que solo hace una o dos pequeñas cosas simples y no sabe nada sobre cómo imprimirse en una consola; esa parte siempre se puede programar más tarde, fuera de la definición de la función.

### <a id="loops" href="#loops">#</a> Loops (Bucles)

Ahora que tenemos algunas habilidades básicas en nuestro haber ( Nota del autor: ¿los gatos incluso usan cinturones? ) Podemos comenzar a ser flojos. ¡¿Qué?! Sí, es cierto: la programación se trata de ser flojo. Larry Wall, inventor del lenguaje de programación Perl, calificó la pereza como la [virtud más importante](http://c2.com/cgi/wiki?LazinessImpatienceHubris) de un buen programador. Si no existieran las computadoras, tendrías que hacer todo tipo de tareas tediosas a mano, pero si aprendes a programar puedes ponerte al sol todo el día mientras una computadora en algún lugar ejecuta tus programas por ti. ¡Es un estilo de vida glorioso lleno de relajación!

Los bucles son una de las formas más importantes de aprovechar el poder de una computadora. ¿Recuerdas `Underscore.js` de antes? Asegúrese de tenerlo cargado en la página (recuerde: puede presionar la flecha hacia arriba en su teclado varias veces y luego presionar `Enter` para cargarlo nuevamente si es necesario) e intente copiar / pegar esto en su consola:
  
```js
function logANumber(someNumber) {
  console.log(someNumber)
}
_.times(10, logANumber)
```

Este código usa el [times](http://underscorejs.org/#times) método de tiempos de subrayado que toma 1 número y 1 función y luego comienza desde 0 y para 10 pasos cuenta hasta 1, llamando a la función con el número en cada paso del camino.

![console](images/times-loop.png)

Si escribiéramos manualmente lo que `times` está haciendo en el código anterior, se vería así:

```js
logANumber(0)
logANumber(1)
logANumber(2)
logANumber(3)
logANumber(4)
logANumber(5)
logANumber(6)
logANumber(7)
logANumber(8)
logANumber(9)
```

Pero los gatos se niegan a hacer trabajos manuales innecesarios como este, por lo que siempre debemos preguntarnos: _"¿Estoy haciendo esto de la manera más perezosa posible?"_ .

Entonces, ¿por qué esto se llama bucle? Piénselo así: si escribiéramos una lista de 10 números (del 0 al 9) usando una matriz de JavaScript, se vería así:

```js
var zeroThroughTen = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

Lo que `times` realmente hace es visitar cada número y repetir una tarea: en el ejemplo anterior, la tarea era llamar a la `logANumber` función con el número actual. Las tareas repetidas de esta manera se denominan _bucles sobre?_ la matriz.

### <a id="arrays" href="#arrays">#</a> Arrays

Lo he mencionado algunas veces, pero pasemos un minuto aprendiendo sobre ellos. Imagina que necesitas hacer un seguimiento de todos tus amigos. Bueno, una matriz funcionará bien. Piense en una matriz como una lista ordenada en la que puede guardar toneladas de cosas.

Así es como haces uno:

```js
var myCatFriends = ["bill", "tabby", "ceiling"]
```

¡Dulce! Ahora tienes una lista de tus amigos gatos.

Los elementos (que es lo que llama un solo elemento en una matriz) que se almacenan dentro de las matrices comienzan en 0 y cuentan desde allí. Entonces `myCatFriends[0]` vuelve `bill` y `myCatFriends[1]` vuelve `tabby`... etc. etc.

Para sacar amigos de su nuevo Array, simplemente puede acceder a un elemento directamente de esta manera:

```js
console.log(myCatFriends[0])
```

![console](images/array-access.png)

Si ha realizado un nuevo gato amigo en el club más de moda gato la otra noche y desea agregar a su lista es muy simple: `myCatFriends.push("super hip cat"`).

Para verificar que el nuevo gato haya llegado a su matriz, puede usar `.length`:

![console](images/array-push-length.png)

Observe cómo pushdevuelve la longitud? ¡Práctico! También tenga en cuenta que las matrices siempre **conservarán el orden**, lo que significa que recordarán el orden en que agregó o definió las cosas. No todo en JavaScript conserva el orden, así que recuerda esta propiedad especial de las matrices.

### <a id="objects" href="#objects">#</a> Objects

Las matrices son buenas para las listas, pero para otras tareas pueden ser difíciles de trabajar. Considera nuestra variedad de amigos gatos. ¿Y si también quisieras almacenar más que solo nombres?

```js
var myCatFriends = ["bill", "tabby", "ceiling"]
var lastNames = ["the cat", "cat", "cat"]
var addresses = ["The Alley", "Grandmas House", "Attic"]
```

A veces es bueno tener todas las direcciones o nombres en una variable. Pero a veces tienes un gato en mente, digamos Bill, y solo quieres buscar la dirección de ese gato. Con las matrices se necesita mucho trabajo porque no se puede decir simplemente 'oye matriz, dame la dirección de Bill' porque 'Bill' está en una matriz y su dirección está en una matriz totalmente diferente.

![console](images/array-lookup.png)

¡Esto puede ser frágil porque si nuestras matrices cambian y agregamos un nuevo gato al principio, también tendríamos que actualizar nuestra `billsPosition` variable para apuntar a la nueva ubicación de la información de `Bill` en las matrices! Aquí hay una manera más fácil de mantener la información de esta manera mediante objetos:

```js
var firstCat = { name: "bill", lastName: "the cat", address: "The Alley" }
var secondCat = { name: "tabby", lastName: "cat", address: "Grandmas House" }
var thirdCat = { name: "ceiling", lastName: "cat", address: "Attic" }
```
  
¿Por qué lo haríamos de esta manera? Porque ahora tenemos una variable para cada gato que podemos usar para obtener los valores de esos gatos de una manera más conveniente y fácil de leer.

![console](images/object-lookup.png)

Puedes pensar en los objetos como llaves en un llavero. Cada uno es para una puerta específica y si tiene buenas etiquetas en sus llaves, puede abrir puertas muy rápido. De hecho, las cosas en el lado izquierdo de la `:` se llaman **kyes** claves (también se conocen como **propiedades** ) y las cosas en el lado derecho son **valores** .

```js
// an object with a single key 'name' and single value 'bill'
{ name: 'bill' }
```

Puedes pensar en los objetos como llaves en un llavero. Cada uno es para una puerta específica y si tiene buenas etiquetas en sus llaves, puede abrir puertas muy rápido. De hecho, las cosas en el lado izquierdo de la :se llaman claves (también se conocen como propiedades ) y las cosas en el lado derecho son valores .

```js
{ date: "10/20/2012", diary: "slept a bit today", name: "Charles" }
```

Pero la computadora podría devolvérselo así:


```js
{ diary: "slept a bit today", name: "Charles", date: "10/20/2012" }
```

¡O así!


```js
{ name: "Charles", diary: "slept a bit today", date: "10/20/2012" }
```

Por lo tanto, nunca puede confiar en el orden de las claves en los objetos. Si quieres REALMENTE elegante, puedes hacer una matriz llena de objetos, ¡o un objeto lleno de matrices!


```js
var moodLog = [
  {
    date: "10/20/2012",
    mood: "catnipped"
  }, 
  {
    date: "10/21/2012",
    mood: "nonplussed"
  },
  {
    date: "10/22/2012",
    mood: "purring"
  }
]

// ordered from least to most favorite
var favorites = {
  treats: ["bird sighting", "belly rub", "catnip"],
  napSpots: ["couch", "planter box", "human face"]
}
```

Cuando combina diferentes cosas como esta, está creando **estructuras de datos** , ¡al igual que los legos!


### <a id="callbacks" href="#callbacks">#</a> Callbacks

Las devoluciones de llamada no son realmente una característica de JavaScript como `Object` o `Array`, sino solo una cierta forma de usar funciones. Para comprender por qué las devoluciones de llamada son útiles, primero debe aprender sobre la programación asincrónica (a menudo abreviada a asíncrona). El código asíncrono por definición es un código escrito de una manera que no es síncrona. El código sincrónico es fácil de entender y escribir. Aquí hay un ejemplo para ilustrar:
```js
var photo = download('http://foo-chan.com/images/sp.jpg')
uploadPhotoTweet(photo, '@maxogden')
```

Este synchronous [pseudo-code](http://simple.wikipedia.org/wiki/Pseudocode) descarga una adorable foto de gato y luego sube la foto a Twitter y tuitea la foto en `@maxogden`. ¡Muy claro!

(*Author's note: I @maxogden do happily accept random cat photo tweets*)

Este código es sincrónico porque para que la foto se cargue en el tweet, la descarga de la foto debe completarse. Esto significa que la línea 2 no puede ejecutarse hasta que la tarea en la línea 1 haya finalizado totalmente. Si tuviéramos que implementar este pseudocódigo, querríamos asegurarnos de que `download` la ejecución 'bloqueada' hasta que finalizara la descarga, lo que significa que evitaría que se ejecute cualquier otro JavaScript hasta que finalice, y luego cuando la descarga se complete -bloquea la ejecución de JavaScript y la línea 2 se ejecutará.

El código síncrono está bien para cosas que suceden rápido, pero es horrible para cosas que requieren guardar, cargar, descargar o cargar. ¿Qué sucede si el servidor desde el que está descargando la foto es lento, o la conexión a Internet que está usando es lenta, o la computadora en la que está ejecutando el código tiene demasiadas pestañas de video de gato de YouTube abiertas y funciona lentamente? Significa que potencialmente podría tomar minutos de espera antes de que la línea 2 comience a funcionar. Mientras tanto, debido a que se bloquea la ejecución de todo JavaScript en la página mientras se realiza la descarga, la página web se congelaría por completo y dejaría de responder hasta que se complete la descarga.

El bloqueo de la ejecución debe evitarse a toda costa, especialmente cuando hacerlo hace que su programa se congele o deje de responder. Supongamos que la foto de arriba tarda un segundo en descargarse. Para ilustrar cuánto dura un segundo para una computadora moderna, aquí hay un programa que prueba para ver cuántas tareas puede procesar JavaScript en un segundo.

```js
function measureLoopSpeed() {
  var count = 0
  function addOne() { count = count + 1 }

  // Date.now() returns a big number representing the number of
  // milliseconds that have elapsed since Jan 01 1970
  var now = Date.now()

  // Loop until Date.now() is 1000 milliseconds (1 second) or more into
  // the future from when we started looping. On each loop, call addOne
  while (Date.now() - now < 1000) addOne()
  
  // Finally it has been >= 1000ms, so let's print out our total count
  console.log(count)
}

measureLoopSpeed()
```

Copy-paste the above code into your JavaScript console and after one second it should print out a number. On my computer I got `8527360`, approximately **8.5 million**. In one second JavaScript can call the `addOne` function 8.5 million times! So if you have synchronous code for downloading a photo, and the photo download takes one second, it means you are potentially preventing 8.5 million operations from happening while JavaScript execution is blocked.

Algunos idiomas tienen una función llamada sleepque bloquea la ejecución durante algunos segundos. Por ejemplo, aquí hay un[`bash`](http://en.wikipedia.org/wiki/Bash_%28Unix_shell%29) código que se ejecuta en`Terminal.app` en Mac OS que usa `sleep`. Cuando ejecuta el comando, `sleep 3 && echo 'done sleeping now'` se bloquea durante 3 segundos antes de imprimir `done sleeping now`.

![console](images/bash-sleep.png)

JavaScript no tiene una `sleep`functión. Como eres un gato, probablemente te estés preguntando: "¿Por qué estoy aprendiendo un lenguaje de programación que no implica dormir?". Pero quédate conmigo. En lugar de `sleep` esperar a que sucedan cosas, el diseño de JavaScript fomenta el uso de funciones. Si tiene que esperar a que termine la tarea A antes de realizar la tarea B, coloca todo el código de la tarea B en una función y solo llama a esa función cuando A finaliza.

Por ejemplo, este es un código de estilo de bloqueo:

```js
a()
b()
```

Y esto está en un estilo sin bloqueo:

```js
a(b)
```

En la versión sin bloqueo `b` es un `callback` a `a` . En la versión de bloqueo `a` y `b` son ambos llamados(called) / invocado (ambos tienen `()` detrás de ellos, que ejecuta las funciones de inmediato). En la versión sin bloqueo, notará que solo `a` se invoca, y `b` simplemente se pasa `a` como argumento.

En la versión de bloqueo, no hay una relación explícita entre `a` y `b`. En la versión sin bloqueo, se convierte en `a` el trabajo de hacer lo que tiene que hacer y luego llamar `b` cuando haya terminado. El uso de funciones de esta manera se denomina devoluciones de llamada porque su función de devolución de llamada, en este caso `b`, se llama más tarde cuando `a` todo está listo.

Aquí hay una implementación de pseudocódigo de lo que `a` podría ser:

```js
function a(done) {
  download('https://pbs.twimg.com/media/B4DDWBrCEAA8u4O.jpg:large', function doneDownloading(error, png) {
    // handle error if there was one
    if (err) console.log('uh-oh!', error)
    
    // call done when you are all done
    done()
  })
}
```

Piense en nuestro ejemplo sin bloqueo `a(b) `, donde llamamos `a` y pasamos `b` como primer argumento. En la definición de la función `a` anterior, el `done` argumento es nuestra `b` función que transmitimos. Este comportamiento es algo difícil de entender al principio. Cuando llamas a una función, los argumentos que pasas no tendrán los mismos nombres de variables cuando estén en la función. En este caso, lo que llamamos `b`se llama donedentro de la función. Pero `b` y `done` son solo nombres de variables que apuntan a la misma función subyacente. Por lo general, las funciones de devolución de llamada se etiquetan como `done` o `callback` para dejar en claro que son funciones que deberían llamarse cuando se realiza la función actual.

Por lo tanto, siempre `a` que sea su trabajo y se llame `b` cuando se hace, ambos `a` y `b` recibir llamadas en las versiones de bloqueo y no bloqueo. La diferencia es que en la versión sin bloqueo no tenemos que detener la ejecución de JavaScript. En general, el estilo sin bloqueo es donde escribe todas las funciones para que pueda regresar lo antes posible, sin bloquear.

Para llevar el punto a casa aún más: si `a` tarda un segundo en completarse y usa la versión de bloqueo, significa que solo puede hacer una cosa. Si usa la versión sin bloqueo (también conocida como devoluciones de llamada), puede hacer _literalmente millones_ de otras cosas en ese mismo segundo, lo que significa que puede terminar su trabajo millones de veces más rápido y dormir el resto del día.

Recuerde: la programación tiene que ver con la pereza y usted debe ser el que duerme, no su computadora.

Espero que ahora pueda ver que las devoluciones de llamada son solo funciones que llaman a otras funciones después de una tarea asincrónica. Ejemplos comunes de tareas asincrónicas son cosas como leer una foto, descargar una canción, subir una imagen, hablar con una base de datos, esperar que un usuario presione una tecla o haga clic en alguien, etc. Cualquier cosa que lleve tiempo. JavaScript es realmente excelente para manejar tareas asincrónicas como estas siempre y cuando se tome el tiempo de aprender a usar devoluciones de llamada y evitar que su JavaScript sea bloqueado.

## The end!

¡Esto es solo el comienzo de su relación con JavaScript! No puedes aprenderlo todo de una vez, pero debes encontrar lo que funciona para ti y tratar de aprender todos los conceptos aquí.

¡Recomiendo volver mañana y revisar todo desde el principio! Puede pasar varias veces antes de obtener todo (la programación es difícil). Solo trate de evitar leer esta página en cualquier habitación que contenga objetos brillantes. . . Pueden ser increíblemente molestos.

¿Tienes otro tema que quieres ver cubierto? Abre un problema [en github](http://github.com/maxogden/javascript-for-cats).

### <a id="recommended-reading" href="#recommended-reading">#</a> Recommended reading

 JavaScript For Cats omite muchos detalles que no son importantes para comenzar (los gatos no son conocidos por su capacidad de atención), pero si siente que necesita profundizar más, consulte estos:
  
  - [NodeSchool.io](http://nodeschool.io/)es un software educativo de código abierto impulsado por la comunidad que enseña varias habilidades de desarrollo web en un formato interactivo y autoguiado. ¡Ayudé a hacer NodeSchool! Lamentablemente, presenta menos gatos que esta página. 
  
  - [Eloquent Javascript](http://eloquentjavascript.net/) es un libro gratuito que te enseña JavaScript! ¡Es bastante bueno! Especialmente el capítulo sobre  [values, variables, and control flow](http://eloquentjavascript.net/chapter2.html)
  - [Mozilla's JavaScript Guide](https://developer.mozilla.org/en-US/docs/JavaScript/Guide) also has a pretty sweet intro chapter called [values, variables and literals](https://developer.mozilla.org/en-US/docs/JavaScript/Guide/Values,_variables,_and_literals)
  - [`standard` JS Style Guide](https://github.com/feross/standard) is a "zero configuration" linter for JS style that I use
  - [Let's Write Code by @shama](https://github.com/shama/letswritecode) a great series of YouTube coding tutorials made by a friend of mine

<hr>
### <a id="satisfied-customers" href="#satisfied-customers">#</a> Satisfied customers
<center>![satisfied customer](images/customers5.jpg)</center>
<center>![satisfied customer](images/customers1.png)</center>
<center>![satisfied customer](images/customers2.png)</center>
<center>![satisfied customer](images/customers3.png)</center>
<center>![satisfied customer](images/customers4.png)</center>

*JSForCats.com is a labor of love and work in progress by [@maxogden](http://twitter.com/maxogden). If you would like to contribute and make this tutorial better there is a Github repo [right over here](http://github.com/maxogden/javascript-for-cats).*
<center>![console](images/awesome.jpg)</center>
