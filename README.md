# trivia.5.2
Repositorio de procesos de creación y construcción del proyecto de Trivia para la ore-admisión de Laboratorio

<h2>DÍA #1:</h2>
El proceso creativo de la construcción de la primera versión de la Webapp "Triviart" comenzó con un proceso de ideación de las pantallas, textos, mensajes, estructura y temas que pudieran configurar el MPV como entregable.

Día #2:
En base a los tres prototipos del proyecto, el equipo definió las características y los atributos más viables de las tres propuestas teniendo clara una versión A más simplificada y en caso de tener tiempo para trabajar, completar una versión B más ambiciosa.

Después de una charla con Carlos (coach) se decidió que el proyecto de trivia priorizaría la funcionalidad y la estructura, dejando en una segunda capa de trabajo el estilo y diseño.

Se trabajó de manera sencilla una guía de estilo que incluye: tipografías, colores, una propuesta de logo y diseño de botones.

Link a guía de estilo: https://www.figma.com/file/gJDAsWhz7sF9r0J3CdjeCk/TriviArt?node-id=0%3A1

Después del primer día de trabajo en el proyecto, dividimos las tareas en partes iguales para poder avanzar en tres canales diferentes durante la tarde y así comenzar el segundo día con avances grandes para que todo el equipo pudiera trabajar en los detalles y/o dificultades con las que cada integrante se enfrentó en su proceso individual.

Se adjunta link de video del resultado del día 1: https://youtu.be/FEYRUSvCnb0


Día #3:
Comenzamos presentando avances de manera grupal. Identificamos los siguiente:

*Hasta este momento nuestro proyecto era funcional sólo a través de enlaces entre archivos HTML
*Era necesario trabajar el código de JS para hacerlo dinámico desde ahí

Invertimos este día para trabajar en conjunto en temas de funcionalidad desde JS. Investigamos y nos perdimos mucho pero logramos un primer ejercicio de escribir un condicional, aunque no corría porque seguramente tenía errores:

/*PRUEBAS KARLA*/

const respuestaIncorrecta = ["incisoA", "incisoC", "incisoD"];
const respuestaCorrecta = ["incisoB"];

  if (respuestaCorrecta == true) {
    document.write ("¡Felicidades! Sí que conoces de Arte")

  } else {
    document.write ("¡OH! Intenta probar más suerte en la siguiente pregunta")
  }
  
  
Durante la tarde cada uno hizo un proceso de investigación y pruebas de condicionales para evaluar las respuestas de la trivia y sobre la creación de botones desde JS:

*PRUEBAS CECI*/

/*crear botones con JS*/
const button = document.createElement('button'); 
  button.type = 'button'; 
  button.innerText = 'Arte Pictórico'; 
  document.body.appendChild(button); 

function botones(){
  document.querySelector(categoriaA){
    if (categoriaA) 
  }


function crearboton(){
   //aquí instanciamos al componente padre
   const categorias = document.getElementById("categorias");
   //aquí agregamos el componente de tipo input
   var input = document.createElement("INPUT");
   //aquí indicamos que es un input de tipo text
   input.type = 'text';
   
   //y por ultimo agreamos el componente creado al padre
   padre.appendChild(input);
 }
 
 
 
 Día #3:

Compartimos hallazgos en equipo. Identificamos lo siguiente:

*Karla había avanzado en la creación de preguntas como archivos HTML enlazados :)
*Saraí había encontrado una manera de evaluar las respuestas desde JS!!! Yupi!
*Ceci había avanzando en el estilo de la página y había probado crear botones desde JS.
*La página ya tenía mejor vista y eso nos inspiraba un poco más :)


Decidimos ir con el trozo de código de Saraí para intentar crear un nuevo Real.it que probara la ruta de JS, sin destruir nuestro entregable del día anterior que se construyó con enlaces de HTML:

function evaluetaAnswer(event) {
  const identifier = event.target.id /
    
    if(identifier === "optionC") {
      document.getElementById(identifier).classList.add('goodAnswer')
      setTimeout(function(){
        location.href="https://www.google.com"
      },5000)
    } else {
      		document.getElementById(identifier).classList.add('wrongAnswer')
          /*document.getElementById("optionC").classList.add('goodAnswer')*/
      setTimeout(function(){
        location.href="https://www.google.com"
      },5000)
    }
  }


  document.getElementById('optionA').addEventListener ('click',evaluetaAnswer)
  document.getElementById('optionB').addEventListener ('click',evaluetaAnswer)
  document.getElementById('optionC').addEventListener ('click',evaluetaAnswer)
  document.getElementById('optionD').addEventListener ('click',evaluetaAnswer)
  
  
  
ENLACES A REPL.IT: 
  
Enlace a Repl.it de ejercicio con la ruta de condicionales: ttps://repl.it/@CeciliaLosada/TriviArtJS#index.html

Enlace a Repl.it de ejercicio con enlaces de HTML: https://repl.it/@CeciliaLosada/TRIVIASQUAD-52#index.html


