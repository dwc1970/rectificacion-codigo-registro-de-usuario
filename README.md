# rectificacion-codigo-registro-de-usuario
nueva rectificacion en el codigo fuente de formulario de usuario

git branch -m main rectificaciones-de-formulario
git buscar origen
git branch -u origin/rectifiacaciones-de-formulario rectificaciones-de-formulario
git remoto set-head origen -a

<!DOCTYPE html> 
<html>
<head>
<meta charset="utf-8" />
<title>Formulario para darse de Alta</title> 
<style type="text/css">
/* Características generales de la página */
body {
  font-size: 14px;
  font-family: Arial, sans-serif;
  background: #AAA;
}

/* El contenedor define la zona principal de contenido */
#contenedor {
  background: #FFF;
  margin: 1em auto;
  padding: 1em;
  width: 768px;
}

/* El formulario está definido como una lista */
ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

ul li {
  border-top: 1px solid #CCC;
  margin: 1em 0;
  padding: 1em;
  width: auto;
  overflow: hidden;
}

/* El formulario se organiza en dos columnas, el título y los controles */
ul li label.titulo {
  float: left;
  width: 150px;
  text-align: right;  
}
 
ul li div.controles {
  margin-left: 160px;
}

/* El último elemento del formulario es el botón "Registrarse" */
ul li.botones {
  border-top: 2px solid #CCC;
  clear: both;
  float: none;
  padding: 1em 0;
  text-align: right;
  width: 100%;
}
 
ul li.botones input {
  font-size: 18px;
}

/* El título de los elementos de la lista */ 
ul li label.titulo {
  font-weight: bold;
}
 
ul li div span {
  float: left;
  padding: 0.3em 0;
}
 
ul li div span.completo {
  width: 100%;
}
 
ul li div span.mitad {
  width: 50%;
}
 
ul li div span.tercio {
  width: 33%;
}
 
ul li div span.dostercios {
  width: 66%;
}

/* Como se define display: block, se muestra en la línea siguiente */
ul li div span label {
  display: block;
  font-size: 12px;
  color: #333;
}

/* Configuración de los controles del formulario */
ul li input {
  padding: 0.2em;
}
 
input#apellido1, input#apellido2, input#direccion, input#email {
  width: 260px;
}
 
input#codigopostal {
  width: 80px;
}
 
select#provincia {
  width: 90px;
}
 
select#pais {
  width: 150px;
}
 
input#telefonofijo, input#telefonomovil {
  width: 135px;
}
 
/* Cambia el color cuando se sitúa el cursor del ratón */
ul li:hover {
  background-color: #FF9;
}
 
ul li.botones:hover {
  background-color: transparent;
}

/* Destaca el control cuando recibe el foco */
ul li input, ul li select {
  border: 2px solid transparent;
  border-bottom: 2px solid black;
}

ul li.botones input {
  border: 2px solid #CCC;
}

ul li input:focus, ul li select:focus {
  border: 2px solid #F00;
}
</style>
</head>
 
<body>
<div id="contenedor">
 
<h1>Formulario de registro</h1>
 
<form method="post" action="#">
<ul>
<li>
  <label class="titulo" for="nombre">Nombre y apellidos</label>
  
  <div class="controles">
    <span class="completo">
      <input id="nombre" name="nombre" value="" />
      <label for="nombre">Nombre</label>
    </span>
 
    <span class="completo">
      <input id="apellido1" name="apellido1" value="" />
      <label for="apellido1">Apellido</label>
    </span>
 
   
  </div>
</li>
 
<li>
  <label class="titulo" for="direccion">Dirección</label>
 
  <div class="controles">
    <span class="completo">
      <input id="direccion" name="direccion" value="" />
      <label for="direccion">Calle, número, piso, puerta</label>
    </span>
 
    <span class="tercio">
      <input id="codigopostal" name="codigopostal" value="" />
      <label for="codigopostal">Código postal</label>
    </span>
 
    <span class="dostercios">
      <input id="municipio" name="municipio" value="" />
      <label for="municipio">Municipio</label>
    </span>
 
    <span class="tercio">
      <select id="provincia" name="provincia">
        <option value=""></option>
        <option value="provincia1">Mendoza</option>
        <option value="provincia2">San Luis</option>
        <option value="provincia3">Tucuman</option>
        <option value="provincia3">La Rioja</option>
        <option value="provincia3">San Juan</option>
        <option value="provincia3">Cordoba</option>
        <option value="provincia3">Catamarca</option>
        <option value="provincia3">Buenos Aires</option>
        <option value="provincia3">Salta</option>
        <option value="provincia3">Tierra del Fuego</option>
        <option value="provincia3">Jujuy</option>
        <option value="provincia3">Santiago del Estero</option>
        <option value="provincia3">Formosa</option>
        <option value="provincia3">Neuquen</option>
        <option value="provincia3">Chubut</option>
        <option value="provincia3">Santa Fe</option>
        <option value="provincia3">Entre Rios</option>
        <option value="provincia3">Chaco</option>
        <option value="provincia3">Corrientes</option>
        <option value="provincia3">Santa Cruz</option>
        <option value="provincia3">Rio Negro</option>
        <option value="provincia3">La Pampa</option>
        <option value="provincia3">Misiones</option>
        <option value="provincia3">C.a.b.a</option>
      </select>
      <label for="provincia">Provincia</label>
    </span>
 
    <span class="dostercios">
      <select id="pais" name="pais">
        <option value=""></option>
        <option value="pais1">Argentina</option>
        <option value="pais2">Chile</option>
        <option value="pais3">Bolivia</option>
      </select>
      <label for="pais">País</label>
    </span>
  </div>
</li>
 
<li>
  <label class="titulo" for="email">Email</label>
 
  <div class="controles">
    <span class="completo">
      <input id="email" name="email" value="" />
    </span>
  </div>
</li>
 
<li>
  <label class="titulo" for="telefonofijo">Teléfono</label>
 
  <div class="controles">
    <span class="mitad">
      <input id="Codigo Area" name="Codigo Area" value="" />
      <label for="Codigo Area">Fijo</label>
    </span>
 
    <span class="mitad">
      <input id="telefonomovil" name="telefonomovil" value="" />
      <label for="telefonomovil">Celular</label>
    </span>
  </div>
</li>
 
<li class="botones">
  <input id="alta" type="submit" value="Registrarse" href="file:///C:/Users/eliza/Desktop/Sabado/registro_2.html.html" target="_blank">
   
  <li><a href="mailto:miusuario@miemail.com" target="_blank">Registrarse</a></li>
  <a href=""></a>
  
      <button class="b-btn-l" type="submit" name="send" value="wnd_FormBlock_467041949">
				<span class="text b-btn-t">Enviar</span>
			</button>
    </button>
  </div>
</div>

</li>
 
</ul>
</form>
 
</div>

</body>
</html>
