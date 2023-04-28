# Curso de fundamentos de Sass en Platzi

## Recursos
- [Documentación de Sass](https://sass-lang.com/documentation/)
- [Landing en Platzi](https://anamdiazs.github.io/eco-store-platzi/)
- [Maquetado del proyecto en Figma](https://www.figma.com/file/Em1aDiIHmqozHpUAjsYhT7/Eco-Store-Mockups-(Copy)?node-id=0-1&t=XnwZpdCNaYggBsGh-0)
- [Fuente del proyecto](https://fonts.google.com/specimen/IBM+Plex+Sans?query=ibm+plex+sans)

# Anotaciones sobre el curso
## ¿Qué son y cómo funcionan los preprocesadores?

Un preprocesador es una herramienta que nos permite escribir pseudocódigo recibiendo como parámetro de entrada los estilos que posteriormente serán convertidos a CSS nativo. Podemos decir que funcionan de manera similar a los traductores pues al indicarle una sintaxis devuelve los valores en una sintaxis nueva.

En SASS se incluyen características adicionales, como variables, mixins, herencia de clases, entre otras, que hacen que el proceso de escritura de CSS sea más fácil y rápido.

Para poder hacer uso de un preprocesador, primero es necesario entender cómo funcionan los estilos CSS y el navegador. Los estilos CSS son interpretados y representados por el navegador, el cual se encarga de leer el código CSS y aplicarlo a los elementos o componentes HTML de la página. Es el navegador quien recorre la hoja de estilos, línea por línea, y asigna propiedades a los elementos de la página según lo indicado en el código CSS. Este proceso es fundamental para permitir que la página se estilice de la manera deseada, teniendo control sobre el diseño y la disposición de la página, proporcionando al usuario una experiencia visual atractiva, donde todos los elementos están estilizados y presentados de una manera agradable a la vista y fácil de interactuar.

## Ventajas de utilizar un Preprocesador

Los principales beneficios de usar un preprocesador como SASS son la rapidez y la productividad. Permitiendo que el código se pueda escribir de manera mucho más rápida y sencilla, ayudando a los desarrolladores a ahorrar tiempo y ser más productivos. También hacen que el mantenimiento del código sea más fácil, pues todos los estilos se guardan en un solo archivo. La reutilización de código es otro de los beneficios que nos trae el uso de un preprocesador, esto significa que los mismos estilos se pueden aplicar en varias páginas sin tener que escribir el código una y otra vez.
Finalmente el uso de preprocesadores nos permite que sea mucho más sencillo trabajar una página web de manera responsiva.

# Estructuras de ls hojas de estilos en Sass
Algunos statements contienen bloques y se definen entre un par de llaves {}, son separados mediante punto y coma ;

## Top level statements
Son declaraciones que solo se pueden utilizar en la parte superior de la hoja como:
- Imports
- Definición de un Mixin
- Definición de función
- Módulos

## Variables
Un espacio asignado en memorias que solo guarda un dato. Estas pueden ser declaradas en cualquier lugar de la hoja de estilos.

Para inicializar una variable se usa el signo $ al principio:

<pre>
  <code>
    $primary-color: blue;
    $secondary-color: green;
    $tertiary-color: purple;
  </code>
</pre>

### Variables CSS
- Pueden tener diferentes valores para distintos elementos.
- Son declarativas.

### Variables Sass
- Tienen un valor único, correspondientes a un elemento.
- Son imperativas.

### !default flag
Se encarga de asignar un valor a la variable si y solo si esta variable no está definida o su valor es null.

### Shadowing
Las variables locales y globales pueden tener el mismo nombre siempre y cuando tengan un alcance o scope distinto.

### !global flag
Permite cambiar el scope de una variable local a global.

