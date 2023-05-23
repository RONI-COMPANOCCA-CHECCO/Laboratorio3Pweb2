<div align="center">
<table>
    <theader>
        <tr>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/epis.png?raw=true" alt="EPIS" style="width:50%; height:auto"/></td>
            <th>
                <span style="font-weight:bold;">UNIVERSIDAD NACIONAL DE SAN AGUSTIN</span><br />
                <span style="font-weight:bold;">FACULTAD DE INGENIERÍA DE PRODUCCIÓN Y SERVICIOS</span><br />
                <span style="font-weight:bold;">DEPARTAMENTO ACADÉMICO DE INGENIERÍA DE SISTEMAS E INFORMÁTICA</span><br />
                <span style="font-weight:bold;">ESCUELA PROFESIONAL DE INGENIERÍA DE SISTEMAS</span>
            </th>
            <td><img src="https://github.com/rescobedoq/pw2/blob/main/abet.png?raw=true" alt="ABET" style="width:50%; height:auto"/></td>
        </tr>
    </theader>
    <tbody>
        <tr><td colspan="3"><span style="font-weight:bold;">Formato</span>: Guía de Práctica de Laboratorio</td></tr>
        <tr><td><span style="font-weight:bold;">Aprobación</span>:  2022/03/01</td><td><span style="font-weight:bold;">Código</span>: GUIA-PRLD-001</td><td><span style="font-weight:bold;">Página</span>: 1</td></tr>
    </tbody>
</table>
</div>

<div align="center">
<span style="font-weight:bold;">GUÍA DE LABORATORIO</span><br />
</div>


<table>
<theader>
<tr><th colspan="6">INFORMACIÓN BÁSICA</th></tr>
</theader>
<tbody>
<tr><td>ASIGNATURA:</td><td colspan="5">Programación Web 2</td></tr>
<tr><td>TÍTULO DE LA PRÁCTICA:</td><td colspan="5">Ajax y NodeJS</td></tr>
<tr>
<td>NÚMERO DE PRÁCTICA:</td><td>03</td><td>AÑO LECTIVO:</td><td>2022 A</td><td>NRO. SEMESTRE:</td><td>III</td>
</tr>
<tr>
<td>FECHA INICIO::</td><td>09-may-2022</td><td>FECHA FIN:</td><td>13-may-2022</td><td>DURACIÓN:</td><td>04 horas</td>
</tr>
<tr><td colspan="6">RECURSOS:
    <ul>
        <li>https://www.w3schools.com/nodejs/nodejs_intro.asp</li>
        <li>https://nodejs.org/en/docs/guides/guía-de-primeros-pasos/</li>
        <li>https://nodejs.dev/learn</li>
        <li>https://www.w3schools.com/js/js_api_fetch.asp</li>
        <li>https://expressjs.com/es/</li>
        <li>https://developer.mozilla.org/es/docs/Web/API/Fetch_API/Using_Fetch</li>
        <li>https://developer.mozilla.org/es/docs/Learn/Server-side/Express_Nodejs/Introducción</li>
    </ul>
</td>
<tr><td colspan="6">DOCENTE:
<ul>
<li>Ing. Anibal Sardon</li>
</ul>
</td>
</<tr>
<tr><td colspan="6">ALUMNO:
<ul>
<li>Roni Companocca Checco</li>
</ul>
</td>
</<tr>
</tdbody>
</tabla>

#Ajax  y NodeJS

[![ Licencia ][licencia]][archivo de licencia]
[![ Descargas ][descargas]][lanzamientos]
[![ Última confirmación ][última confirmación]][lanzamientos]

[![ Debian ][Debian]][sitio de Debian]
[![ Git ][Git]][git-sitio]
[![ GitHub ][GitHub]][sitio de github]
[![ Vim ][Vim]][vim-sitio]
[![ Java ][Java]][sitio Java]

#

##  OBJETIVOS TEMAS Y COMPETENCIAS

###  OBJETIVOS

-    Aprender peticiones asíncronas en JavaScript usando JSON para la comunicación.
-    Programar en BackEnd usando JavaScript.
-    Entender el concepto de promesas y los objetos no bloqueantes

###  TEMAS
- Objetos asíncronos
- Comunicación con POST y GET
- Programación en el backend

<detalles>
<summary>COMPETENCIAS</summary>

- Cc Diseña responsablemente sistemas, componentes o procesos para satisfacer necesidades dentro de restricciones realistas: económicos, ambientales, sociales, políticas, éticas, de salud, de seguridad, fabricación y sostenibilidad.
- Cm Construye responsablemente soluciones siguiendo un proceso adecuado llevando a cabo las pruebas dispuestas a los recursos disponibles del cliente.
- Cp Aplica de forma flexible técnicas, métodos, principios, normas, estándares y herramientas de ingeniería necesarias para la construcción de software e implementación de sistemas de información.

</detalles>

##  CONTENIDO DE LA GUIA

###  MARCO CONCEPTUAL

-    https://www.w3schools.com/nodejs/nodejs_intro.asp
-    https://nodejs.org/en/docs/guides/guía-de-primeros-inicios/
-    https://nodejs.dev/learn
-    https://www.w3schools.com/js/js_api_fetch.asp
-    https://expressjs.com/es/
-    https://developer.mozilla.org/es/docs/Web/API/Fetch_API/Using_Fetch
-    https://developer.mozilla.org/es/docs/Learn/Server-side/Express_Nodejs/Introduction

-    Instalar NodeJS
-    Cree un nuevo proyecto NodeJS.
-    Cree un archivo index.js
    ```sh
    const http = require( ' http ' ) ;
    servidor const = http.createServer (( solicitud , respuesta) => {
        consola.log(solicitud.url);
        respuesta.end("Hola mundo");
    });
    servidor.escucha( 3000 );
    console.log("Escuchando en: http://localhost: 3000 ")
    ```
-    Luego lanza el servidor con :    
    ```sh
    nodo index.js
    ```
-    Note que console imprime en la salida estándar y el cliente sólo recibe el texto “Hola Mundo”. http :// 127 . 0 _ 0 _ 1 : 3000 /
-    El siguiente código modifica algunas líneas para usar un framework llamado express y devolver un archivo index.html
-    Para usar este código debe instalar express con npm : 
    ```sh
    $ npm instalación rápida    
    ```
    ```sh
    const ruta = require('ruta');
    const expreso = require('expreso');
    const aplicación = express();
    aplicación.escucha( 3000 , () => {
        console.log("Escuchando en: http://localhost: 3000 ")
    });
    app.get('/', (solicitud, respuesta) => {
        respuesta.sendFile(ruta.resolve(__dirname, 'index.html' )) ;
    }) ;
    ```
-    Debe crear un archivo index.html en el directorio de su proyecto.
-    Tenga en cuenta que el servidor espera recibir una petición de tipo GET y la URL no contiene el nombre del archivo.

##  EJERCICIO RESUELTO POR EL DOCENTE

-    Cree una aplicación web que ejecute javascript en el cliente (dentro de la carpeta pub) y nodejs en el servidor.
    ```sh
    const ruta = require( ' ruta ' ) ;
    const express = require( ' express ' ) ;
    const app = express ();
    app.use(express.static( ' pub ' )) ;
    aplicación.escucha(3000, () = > {
        console.log( " Escuchando en: http://localhost:3000 " )
    });
    app.get( ' / ' , (solicitud, respuesta) = > {
        respuesta.sendFile(ruta.resolve(__dirname, ' index.html ' )) ;
    }) ;
    ```
-    Cree una aplicación web que realice una petición ajax en el lado del cliente y responda usando nodejs en el lado del servidor.
-    En el lado del servidor :
    ```sh
    const fs = require( ' fs ' )
    const ruta = require( ' ruta ' )
    const express = require( ' express ' )
    aplicación const = expreso ()
    app.use(express.static( ' pub ' ))
    aplicación.escucha(3000, () = > {
        console.log( " Escuchando en: http://localhost:3000 " )
    });
    app.get( ' / ' , (solicitud, respuesta) = > {
        respuesta.sendFile(ruta.resolve(__dirname, ' index.html ' ))
    })
    app.get( ' /recitar ' , (solicitud, respuesta) = > {
        fs.readFile(ruta.resolve(__dirname, ' priv/poema.txt ' ), ' utf8 ' ,
            (err, datos) = > {
                si (err) {
                    consola.error(err)
                    respuesta.estado(500).json({
                        error: ' mensaje '
                    })
                    devolver
                }
                respuesta.json({
                    texto: datos.reemplazar(/ \n /g, ' <br> ' )
                })
            })
        //
    })
    ` ` `
- En el lado del cliente:
    ` ` ` sh
    función  recitar() {
        const url = ' http://localhost:3000/recitar '
        buscar (url). entonces (
            respuesta = >  respuesta.json ()
        ).entonces(
            datos = > {
                document.querySelector( " #poema " ).innerHTML = data.text
            }
        )
    }
    ` ` `
- Si tiene errores lea: https://medium.com/zero-equals-false/using-cors-in-express-cac7e29b005b
- Cree una aplicación que haga peticiones AJAX usando POST a un servidor NodeJS
- En el lado del servidor
    ` ` ` sh
    const fs = require( ' fs ' )
    const ruta = require( ' ruta ' )
    const express = require( ' express ' )
    const bp = require( ' analizador de cuerpo ' )
    const MarkdownIt = require( ' markdown-it ' ),
        md = nuevo MarkdownIt ();
    aplicación const = expreso ()
    app.use(express.static( ' pub ' ))
    aplicación.uso(bp.json ())
    app.use(bp.urlencoded({
        extendido: cierto
    }))
    aplicación.escucha(3000, () = > {
        console.log( " Escuchando en: http://localhost:3000 " )
    })
    app.get( ' / ' , (solicitud, respuesta) = > {
        respuesta.sendFile(ruta.resolve(__dirname, ' index.html ' ))
    })
    app.post( ' / ' , (solicitud, respuesta) = > {
        consola.log(solicitud.cuerpo)
        let markDownText = request.body.text
        consola.log(markDownText)
        let htmlText = md.render(markDownText)
        respuesta.setHeader( ' Tipo de contenido ' , ' aplicación/json ' )
        respuesta.end(JSON.stringify({
            texto: texto html
        }))
    })
    ` ` `
- Note que tanto el tanto GET como POST comparten la misma URL.
- Al lado del cliente
    ` ` ` sh
    recital de función  (texto marcado) {
	const url = ' http://localhost:3000/ '
	datos constantes = {
		texto: marcadoTexto
	}
    consola.log(datos)
	petición constante = {
		método: ' POST ' , // Podría ser GET
		encabezados: {
			' Tipo de contenido ' : ' aplicación/json ' ,
		},
		cuerpo: JSON.stringify(datos),
	}
	http = buscar (url, solicitud)
	http.entonces(
		respuesta = >  respuesta.json ()
	).entonces(
		datos = > {
			document.querySelector( " #htmlCode " ).innerHTML = data.text
		}
        )
    }
    documento.addEventListener( ' DOMContentLoaded ' , función  () {
        const text = document.querySelector( ' #markupText ' )
        document.querySelector( ' #markupForm ' ).onsubmit = () = > {
            recitar(texto.valor)
            devolver  falso ;
        }
    })
    ` ` `
#
## EJERCICIOS PROPUESTOS
- En grupos de 3 a 5 personas implemente una aplicación web que navegue sobre archivos Markdown y permita:
    1. Listas de los archivos Markdown disponibles
    2. Ver el contenido de un archivo Markdown convertido a HTML
    3. Crear nuevos archivos MarkDown y almacenarlos en el servidor
- La comunicación entre el cliente y el servidor tiene que ser usando JSON únicamente.
El cliente debe usar AJAX para sus peticiones
El servidor debe usar NodeJS
Su aplicación debe ser de página única, es decir que sólo habrá un archivo index.html y nada más.
- Si los enlaces provistos en esta guía no le son necesarios, puede revisar códigos en Internet que le ayuden con cosas como ejemplos: listar un directorio en NodeJS ; pero deberá incluir los enlaces correspondientes en sus archivos como comentarios y sólo podrá usar el código de stackoverflow, incluir el código de cualquier otra fuente que esté prohibida y se considerará una actitud deshonesta.
#
## CUESTIONARIO
- En el Ejemplo " Hola Mundo " con NodeJS. ¿Qué pasó con la línea: " Tipo de contenido ….. " ?
- En los ejercicios. ¿En qué lugar debería estar el archivo poema.txt ?
- ¿Entiende la expresión regular en el código y se da cuenta de para qué es útil ?
- Tenga en cuenta que la respuesta del servidor está en formato JSON, ¿Habrá alguna forma de verla directamente ?
#
## REFERENCIAS
- Código JavaScript utilizando el último ECMAScript. Packt Publishing Ltd, 2018.
-Greg Lim. Desarrollo inicial de Node.js, Express y MongoDB. Amazonas, 2019.
- https://www.w3schools.com/nodejs/nodejs_intro.asp
- https://nodejs.org/en/docs/guides/guía-de-primeros-inicios/
- https://nodejs.dev/learn
- https://www.w3schools.com/js/js_api_fetch.asp
- https://expressjs.com/es/
- https://developer.mozilla.org/es/docs/Web/API/Fetch_API/Using_Fetch
- https://developer.mozilla.org/es/docs/Learn/Server-side/Express_Nodejs/Introduction
#
[licencia]: https://img.shields.io/github/license/rescobedoq/pw2 ? label=rescobedoq
[archivo de licencia]: https://github.com/rescobedoq/pw2/blob/main/LICENSE
[descargas]: https://img.shields.io/github/downloads/rescobedoq/pw2/total ? label=Descargas
[lanzamientos]: https://github.com/rescobedoq/pw2/releases/
[última confirmación]: https://img.shields.io/github/last-commit/rescobedoq/pw2 ? label=Último%20Confirmar
[Debian]: https://img.shields.io/badge/Debian-D70A53 ? estilo=para-la-insignia & logo=debian & logoColor=blanco
[sitio de Debian]: https://www.debian.org/index.es.html
[Git]: https://img.shields.io/badge/git-%23F05033.svg ? estilo=para-la-insignia & logo=git & logoColor=blanco
[git-sitio]: https://git-scm.com/
[GitHub]: https://img.shields.io/badge/github-%23121011.svg ? estilo=para-la-insignia & logo=github & logoColor=blanco
[sitio de github]: https://github.com/
[Vim]: https://img.shields.io/badge/VIM-%2311AB00.svg ? estilo=para-la-insignia & logo=vim & logoColor=blanco
[sitio vim]: https://www.vim.org/
[Java]: https://img.shields.io/badge/java-%23ED8B00.svg ? estilo=para-la-insignia & logo=java & logoColor=blanco
[sitio Java]: https://docs.oracle.com/javase/tutorial/
[ ! [Debian][Debian]][sitio de Debian]
[ ! [Git][Git]][git-sitio]
[ ! [GitHub][GitHub]][sitio de github]
[ ! [Vim][Vim]][vim-sitio]
[ ! [Java][Java]][sitio Java]
[ ! [Licencia][licencia]][archivo de licencia]
[ ! [Descargas][descargas]][lanzamientos]
[ ! [Última confirmación][última confirmación]][lanzamientos]