## Objetivo 
El objetivo de este "homework" es que tengan un vistazo de lo que van a estar manejando con react
en la segunda semana del modulo 2.

## Primeros pasos
Nosotros les dejamos el proyecto ya creado (Lo creamos con un comando que es npx create-react-app + el nombre del proyecto) 
Van a tener que hacer un npm install para que se instalen las dependencias (por esta vez vamos a tener instalado el react-router-dom pero en el caso de que no lo tengan luego del npm install, solo tienen que ejecutar npm i react-router-dom)

## Orden sugerido
-LandingPage
-Navbar
-Home
-App (Aca conectarian los dos componentes previos para ver como funciona el routeado)

-MovieCard
-Home (Ahora haríamos el renderizado de la lista)
-DetailedMovie (Extra)
## Recomendaciones

Al comenzar a trabajar, recomendamos que empiecen por los componentes que crean mas simples, por ejemplo la landing page o la navbar. Ya les dejamos creados los componentes, pero sientanse libres de agregar o modificarlos a su gusto.

En el componente App.js, vamos a reemplazar el contenido del DIV por las rutas para empezar a conectar los componentes.

Por ejemplo : <Route path="/movies" render={Movies}>

Checkeen que cada ruta renderice el componente correspondiente.

Recomendamos que en el componente home, rendericen la lista de peliculas, les dejamos una pista de como seria la sintaxis para hacerlo. (Ustedes tienen que pensar el import y la logica)

<div>{movies.map( c => (<MovieCard cover={acavaunaprop} name={acavaunaprop}>))}</div>

En navbar solamente vamos a poner un boton que va a tener un link a la home, en este caso no va a tener funcionalidad pero en aplicaciones mas grandes sirve

Como extra, van a hacer una ruta de detalle de la pelicula, a esta ruta vamos a acceder mediante un Link que se va a generar por cada nombre en la card.
