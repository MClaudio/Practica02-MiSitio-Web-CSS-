# Practica02-MiSitio-Web-CSS-
Programacion Hipermedial
Autor: Claudio maldonado
Fecha: 14/04/2019

1.	Se crea el repositorio en GitHub con el nombre Practica02-MiSitio-Web-CSS-
 
•	Posteriormente se procede a cargar los archivos HTML de la practica 01 anterior realizada en HTML.
 
2.	Se crean los archivos css dentro de la carpeta css para el diseño de dos y tres columnas, así como el archivo que contendrá los archivos generales para todas las páginas.
 
3.	Se crea los estilos generales para todas las paginas estos estilos incliyen el diseño del header, menú, el contenido principal y el footer así también como los estilos para los textos e images a continuación.
•	Estilos generales:
 
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    background-image: url("../imagenes/dynamic-style.png");
}
 
•	Estilos de header:

/**HEADER**/
#cabezera{
    width: 100%;
    background-image: url("../imagenes/portada.png");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    height: 14.1em;
}
#cabezera img{
    width: 10em;
    height: 10em;
    position: relative;
    float: left;
    border-radius: 50%;
    top: 2.2em;
    left: 1em;
    transition: transform 2s ease-out;
}
#cabezera>img:hover{
    transform: rotate(360deg);
}
#cabezera h1{
    text-transform: uppercase;
    font-size: 3em;
    display: block;
    position: relative;
    top: 2em;
    left: 25px;
    color: #1C80FF;
}
 
•	Estilos del menú:

/**NAV**/
nav{
    clear: both;
    margin: 5px;
    background-color: #E6DBC8;
    border: 4px dotted #1C80FF;
    border-radius: 20px;
}
nav ul li a{
    color: #404040;
    text-decoration: none;
    display: block;
    padding: 5px;
    margin: 5px;
    transition: 1s ease all;
}
nav ul li a:hover{
    background-color: #1C80FF;
    color: #FFF;
}
 
•	Estilos para el submenú de navegación entre artículos:

/**BODY SUBMENU**/
#contenido .subMenu{
    border: 4px dotted #1C80FF;
    padding: 10px;
    background-color: #E6DBC8;
}
#contenido .subMenu h2{
    text-transform: uppercase;
}
#contenido .subMenu ul{
    text-align: center;
}
#contenido .subMenu li{
    list-style: none;
    display: inline-block;  
}
#contenido .subMenu a{
    text-decoration: none;
    color: black;
    display: inline-block;
    padding: 5px;
    margin: 5px;
    transition: 1s ease all;
}
#contenido .subMenu a:hover{
    text-decoration: underline;
}
 
•	Estilos para el contenedor contenido y los artículos:

/**BODY**/
body #tituloContenido{
    margin: 10px;
    text-transform: uppercase
}
#contenido{
    padding: 10px;
    background-color: #FFF;
}
#contenido article{
    margin: 10px 0px;
    text-align: justify;
    border-bottom: 4px dotted #1C80FF;
    padding-bottom: 5px;
}
#contenido .subTitulos,h3{
    font-size: 1.5em;
}
#contenido img{
    width: 100%;
}
#contenido img:hover{
    opacity: .8;
}
 
•	Estilo para las tablas:

/**BODY TABLA**/
#contenido table{
    background-color: #E6DBC8;
}
#contenido table,td{
    border: 1px solid #1C80FF;
}
#contenido td{
    padding: 5px;
    text-align: center;
}
 
•	Estilos para los asides:

/**ASIDE 1**/
#extra{
    width: 100%;
    display: inline-block;
}
#extra aside{
    width: 45%;
    margin: 10px;
    float: left;
}
#extra img{
    width: 100%; 
}
#extra img:hover{
    opacity: .7;
    cursor: pointer;
}
/**ASIDE 2**/
.rg{
    width: 100%;
}
.rg img{
    width: 100%;
}

•	Estilo para el footer: 

/**FOOTER**/
footer{
    clear: both;
}
footer{
    text-align: center;
    background-color: #E6DBC8;
    border-top: 4px dotted #1C80FF;
}
footer a{
    text-decoration: none;
    color: #1C80FF;
}
footer a:hover{
    color: #000;
}

4.	Se crea los estilos para el diseño de 2 columnas este diseño se logra con flotar los elementos hacia la izquierda:
 
#menu{
   width: 30%;
   float: left;
}
#contenido{
    width: 65%;
    float: left;
}

#contenido iframe{
    width: 100%;
}
 
5.	Se crea el diseño de 3 columnas también para este diseño se hace uso de los floats para poder flotar los contenedores hacia la izquierda.

#menu{
    width: 24%;
    float: left;
}
#contenido{
    width: 50%;
    float: left;
}

#extra{
    width: 24%;
    float: left;
    background-color: #E6DBC8;
    border: 4px dotted #1C80FF;
    border-radius: 20px;
    margin: 5px;
}

#extra img{
    display: block;
    width: 200%;
}
 
Para lograr que estos elementos floten de manera correcta el contenido principal se encierra dentro de un DIV así también como el los asides se encierra dentro de un DIV para lograr 3 cajas que contienen dentro de ellas elementos y a estas poderles dar el tamaño adecuado para que se posicionen una a lado de otra.

6.	Se crea el archivo HTML que contendrá el formulario como esta comparte todo el contenido básico de las otras páginas solo se evidenciara que dentro del contenido principal se encuentra el formulario para contacto:

<a href="contacto.html">Contacto</a>

7.	Posteriormente se procede a dar estilos al formulario para lograr una vista mas amigable:

/**Formulario**/
#contenido .formulario{
    width: 80%;
    margin-top: 20px;
    text-align: center;
}
#contenido .formulario input{
    width: 100%;
    margin: 10px;
    padding: 10px;
    border: transparent;
    border-bottom: 1px solid #1C80FF;
}
#contenido .formulario input:focus{
    border: 1px solid #1C80FF;
}
#contenido .formulario textarea{
    resize: none;
    width: 100%;
    height: 15em;
    margin: 10px;
    padding: 10px;
    border: 1px solid #1C80FF;
}
#contenido .formulario button{
    width: 40%;
    margin: 10px;
    padding: 10px;
    background: #1C80FF;
    border: none;
    border-radius: 10px;
    text-transform: uppercase;
    color: #FFF;
    font-size: 0.9em;
}
#contenido .formulario button:hover{
    background: #155FBF;
}
#contenido .formulario button:active{
    background: #072040;
}
 
RESULTADO(S) OBTENIDO(S):
Se crea un sitio web mas amigable para el usuario y con css se le da un estilo más ameno a la vista del usuario para esta practica se usó los conceptos de modelo de caja y posicionamiento para lograr crear diseños de 2 y 3 columnas además se implementa un formulario para contacto también se hace uso de la herramienta de GitHub el cual el repositorio se pude ver en el siguiente enlace: https://github.com/MClaudio/Practica02-MiSitio-Web-CSS- 
El resultado de aplicar las hojas de estilo se pude apreciar en la siguiente imagen:
 
