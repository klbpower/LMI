# LMI

Ejemplos para seguir el libro y complementar

#La carpeta base
Con node y la extensión Live Server
http://127.0.0.1:5500/

Puedes trabajar donde quieras
ej. $HOME

Las extensiones .html .htm en Windows/Gnu Linux

#Escribir
Contenido 

#Las etiquetas
<etiqueta>Contenido</etiqueta>
<etiqueta atributo="valor"> Contenido</etiqueta>

Hay etiquetas especiales como br, hr e img, no tienen cierre
con VSC al pinchar te aparece la info en MDN 

https://www.w3.org/community/webed/wiki/Es/Doctypes_y_estilos_de_etiquetado
https://developer.mozilla.org/es/docs/Glossary/HTML5
https://developer.mozilla.org/es/docs/Learn <--- 
https://es.wikipedia.org/wiki/HTML5


#HEAD
https://developer.mozilla.org/es/docs/Web/HTML/Element/head
https://developer.mozilla.org/es/docs/Web/HTML/Element/meta
https://developer.mozilla.org/es/docs/Web/CSS/@charset
https://developer.mozilla.org/es/docs/Web/HTML/Element/title


#BODY
https://developer.mozilla.org/es/docs/Web/HTML/Element/body

#Ejemplo Estructura HTML5
estructuraBase.html

#Las etiquetas
https://developer.mozilla.org/es/docs/Web/HTML/Element/Heading_Elements
h1...h6

https://developer.mozilla.org/es/docs/Web/HTML/Element/p
p
hr
https://developer.mozilla.org/es/docs/Web/HTML/Element/hr
 br
https://developer.mozilla.org/es/docs/Web/HTML/Element/br

#Caracteres especiales 
&nbsp; &aacute; &gt; 

strong vs b 
https://developer.mozilla.org/es/docs/Web/HTML/Element/strong

em  vs i
https://developer.mozilla.org/es/docs/Web/HTML/Element/em


#Las etiquetas se pueden anidar
<strong><em>Contenido</em></strong>


#Bloques generales (en línea y en bloque)
span - en línea - misma línea que necesita el contenido
https://developer.mozilla.org/es/docs/Web/HTML/Inline_elements
div  - en bloque 100% espacio + salto de línea
https://developer.mozilla.org/es/docs/Web/HTML/Block-level_elements

#Bloques específicos en bloque como una caja
body -> header, nav, main, section, article, aside, footer

#Listas
https://developer.mozilla.org/es/docs/Web/HTML/Element/ul
ul o ol
  li
  ej. lista compra, peliculas, videojuegos, 

    type="disc/square/circle"

dl 
https://developer.mozilla.org/es/docs/Web/HTML/Element/dl
  dt - palabra a definir
  dd - definición

#Imágenes
<img src="" alt="" title="">
https://developer.mozilla.org/es/docs/Web/HTML/Element/img

#Figure
https://developer.mozilla.org/es/docs/Web/HTML/Element/figure

Envuelve las imágenes
<figure>
    <img src="" alt="" title="" />
    <figcaption> Contenido </figcaption> -- pie de imágen
</figure>


#Video
<video src="" controls autoplay>
https://developer.mozilla.org/es/docs/Web/HTML/Element/video
</video>

<video controls>
    <source src="*.mp4" type="video/mp4" /> 
    <source src="*.ogg" type="video/ogg" /> 
    No compatible con el vídeo
</video>

https://developer.mozilla.org/es/docs/Web/HTML/Element/audio
<audio src="" controls>
 Esta etiqueta no es compatible
</audio>

iframe carga una página dentro de otra - gmaps
https://developer.mozilla.org/es/docs/Web/HTML/Element/iframe
<iframe src="">
</iframe> --> interesesante allowfullscreen y loading="lazy"

#Enlaces
https://developer.mozilla.org/es/docs/Web/HTML/Element/a
<a href="" target="_blank">Enlace</a>

#Anclas // enlaces internos, mucho texto
<a href="#pie_pagina">Pie de página</a>

<footer id="pie_pagina">
Pie de página <a href="#top">Ir arriba</a>
</footer>

Tablas
<table border="1" summary="Resumen">
<caption></caption>
<thead>
    <th></th>
</thead>
<tbody>
    <th scope=row></th>
    <tr>
        <td></td>
    </tr>
</tbody>
<tfoot>
    <tr>
        <td colspan="2"></td>
    </tr>

</tfoot>
</table>

#Formularios : Introducir información para enviarla 
<form method="" action="">
    <label for="id"> Campo</label>
    <input type="text" name="" id="" placeholder="Sugerencia">

    <label for="url"> url</label>
    <input type="url" name="url" id="url" >
    
    <label for="email"> Email</label>
    <input type="email" name="" id="" >

    <label for="id"> password</label>
    <input type="password" name="" id="" >

    <label for="telefono"> Telefono </label>
    <input type="tel" name="telefono" id="telefono" >

    <label for="tiempo"> Tiempo</label>
    <input type="time" name="tiempo" id="tiempo" >

    <label for="mes"> Mes</label>
    <input type="month" name="mes" id="mes" >

  
    <fieldset>
        <legend>Leyenda</legend>
        <label for="descripcion"> Campo</label>
        <textarea id="descripcion" name="descripcion"></textarea>
    </fieldset>

    <label for="opcion1"> Opcion1</label>
    <input type="radio" name="opcion" id="opcion1" value="opcion1">
    <label for="opcion2"> Opcion2</label>
    <input type="radio" name="opcion" id="opcion2" value="opcion2">

   
    <select>
        <opcion name="opcion" id="opcion1" value="opcion1"> Opcion1</opcion>
        <opcion name="opcion" id="opcion2" value="opcion2"> Opcion2</opcion>
    </select>
    
    <input list="opciones" name="opcionElegida">
    <datalist id="opciones" name="opciones">
        <option value="opcion1">
        <option value="opcion2">
        <option value="opcion3">
    </datalist>

     <label for="opcion1"> Opcion1</label>
    <input type="checkbox" name="opcion" id="opcion1" value="opcion1">
    <label for="opcion2"> Opcion2</label>
    <input type="checkbox" name="opcion" id="opcion2" value="opcion2">


    <label for="numero"> Numero</label>
    <input type="number" name="numero" id="numero">
     <label for="rango"> Numero</label>
    <input type="range" name="rango" id="rango">

    <label for="color"> Color</label>
    <input type="color" name="color" id="color">
     <label for="fecha"> Color</label>
    <input type="date" name="fecha" id="fecha">
     <label for="ficheros"> Color</label>
    <input type="file" name="ficheros" id="ficheros">

    <label for="image"> Color</label>
    <input type="image" src="" name="image" id="image">

    <label for="oculto"> </label>
    <input type="hidden"  name="oculto" id="oculto" value="secreto">

    <label for="buscar"> </label>
    <input type="search"  name="buscar" placeholder="Buscar..." id="buscar" value="secreto">

    <button>Botón</button>
    <input type="submit" value="Enviar" />
    <input type="reset" value="Limpiar" />

    <progress min="1" max=100 value="55"></progress>
    <meter min="1" max=100 value="55"></meter>

    
</form>




