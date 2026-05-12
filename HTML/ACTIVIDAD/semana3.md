Respuestas planteadas en el punto 5 del taller 
-----------------------------------------------------------------------------------------

1. ¿Por qué los enlaces son verdes y no rojos?

Los enlaces aparecen verdes porque en el CSS del ejemplo existe una regla que modifica el color de las etiquetas <a>.
El navegador aplica esa regla y modifica el color de los enlaces.

-----------------------------------------------------------------------------------------

2. Se debe cambiar la propiedad color en el selector de enlaces, en el archivo css.
//
a {
    color: red;
}
//
Con este cambio, todos los enlaces aparecerán en color rojo.

-----------------------------------------------------------------------------------------

3. Al cambiar las etiquetas <ul> y <li> por <div>, el diseño cambia o puede presentar fallos.

ya que el CSS original fue creado para trabajar con listas HTML.
Los selectores usados en el CSS busca principalmente elementos <ul> y <li>, por lo que al reemplazarlos por <div>, algunas reglas ya no se aplican.

Además, las listas tienen estilos y comportamientos propios del navegador, mientras que los <div> son elementos genéricos.

-----------------------------------------------------------------------------------------

4. //
/* NO TOCAR ESTOS ESTILOS */
ul.news {
  list-style: none;
  margin: 0;
  padding: 0;
  font-family: arial;
}
a {
  color: red;
}
ul.news li.news__item {
  padding-top: 1em;
  padding-bottom: 1em;
  padding-left: 10px;
}
ul.news li.news__item + li.news__item {
  border-top: 1px solid #ccc;
}
ul.news li.news__item:nth-child(2n) {
  background: #eee;
}
ul.news li.news__item:last-child {
  border-bottom: 1px solid #ccc;
}
ul.news li.news__item h2.news__item-title {
  margin: 0 0 .25em;
  font-size: 20px;
}
ul.news li.news__item a.news__item-link {
  color: green;
}
/* NO TOCAR ESTOS ESTILOS */

/* Nuevos estilos a partir de esta línea */

.main-header {
  background: #333;
  color: white;
  padding: 20px;
}

.header-title {
  font-size: 24px;
  margin: 0;
}

.header-subtitle {
  font-style: italic;
  opacity: 0.8;
}

.content-area {
  padding: 20px;
  line-height: 1.6;
}

.content-section {
  margin-bottom: 30px;
  border-bottom: 1px solid #ddd;
}

.section-title {
  color: #e74c3c;
}

.main-footer {
  text-align: center;
  font-size: 12px;
  color: #777;
  padding: 10px;
}

//