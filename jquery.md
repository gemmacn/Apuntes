*Jquery*
=========================================
Mejor ponerlo al final del body.

document.querySelector('.box')
document.querySelector('#box')

var box = document.querySelector('#box')


El addEventListener

boxhijo.addEventListener('click',function(){
    console.log('clicked')
})
boxpadre.addEventListener('click',function(){
    console.log('hola q tal')
})


Es mejor asi que usar el onclick de html pq te permite addEventListener linkarlo a diferentes funciones.

Propagación de eventos
(bubbling)primero se ejecuta la funcion en el hijo y luego al padre y siguientes.

box.addEventListener('click',function(event){
    console.log('hola q tal');
    event.stopPropagation();
})

// aqui event se refiere a "click", es un objeto que representa al evento y tiene sus metodos.

boxpadre.addEventListener('click',function(){
    console.log('hola q tal');
},true);
--->al poner este true, el primer evento es el del padre.

Según si hay true o no, el stopPropagation va hacia fuera o hacia dentro.


---------------------------------------------------------------------------------
Como detectar si esta jquery: Con el HTMl abierto en el browser ue tiene linkado el Jquery.
desde la consola pones: $
f(a,b)function ---------------> es que si.



$( ".box" ).click(function() {
  alert( "Handler for .click() called." );
  ('.box')
});













