

**EXPRESS


$ npm install express --save

 app.all(),  no se deriva de ningún método HTTP. 
 Este método se utiliza para cargar funciones de middleware en una vía de acceso para todos los métodos de solicitud.
 (GET, POST, PUT, DELETE)
 
 app.all('/secret', function (req, res, next) {
  console.log('Accessing the secret section ...');
  *next()*; // pass control to the next handler
});


