

#EXPRESS

$ npm install express --save

una aplicación Express es fundamentalmente una serie de llamadas a funciones de middleware.

Las funciones de middleware son funciones que tienen acceso al objeto de solicitud (req), al objeto de respuesta (res) y a la siguiente función de middleware en el ciclo de solicitud/respuestas de la aplicación. La siguiente función de middleware se denota normalmente con una variable denominada next.

Si la función de middleware actual no finaliza el ciclo de solicitud/respuestas, debe invocar next() para pasar el control a la siguiente función de middleware. De lo contrario, la solicitud quedará colgada.


 app.all(),  no se deriva de ningún método HTTP. 
 Este método se utiliza para cargar funciones de middleware en una vía de acceso para todos los métodos de solicitud.
 (GET, POST, PUT, DELETE)
 
 app.all('/secret', function (req, res, next) {
  console.log('Accessing the secret section ...');
  **next()**; // pass control to the next handler
});


** express.static**

app.use(express.static('public'));

app.use('/static', express.static(__dirname + '/public'));

