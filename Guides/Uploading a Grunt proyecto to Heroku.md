##Subir un Proyecto Grunt a Heroku

- Tener Cuenta en Heroku.
- Tener Proyecto Grunt con la carpeta Dist generada `grunt build`
- Installar Express (Framework Node)

```$ npm install express -save```

- Crear un servidor Express si quieres saber mas de express ( http://expressjs.com/guide.html ):
  - crear archivo js en el root de tu proyecto, ejemplo app.js

  ```
  var express = require('express');
  var port = process.env.PORT || 3000;
  var app = express();
  app.use(express.static(__dirname + '/dist'));
  app.listen(port);
  ```
- Crear archivo con el nombre Procfile en el root de tu proyecto que contenga esta linea `web: node app.js`
- Si nunca has subido a heroku has push a Heroku antes de hacer el siguiente paso.
- Agregar un Web Dyno, lo puedes hacer directamente en la pagina de tu proyecto en heroku o con la siguinete linea en consola `$ heroku ps:scale web=1`
- Remueve la Carpeta Dist del gitignore
- Ya puedes hacer push a Heroku