# 0. Presentación
- Tres horas por tema (introducción, configuraciones, ejercicios resueltos por mi, tiempo para hacer ejercicios)
- Aplicaciones Web
- Servicios
- Otros conceptos que he visto en los scripts pero que no son web:
  - OCR
    - https://www.jesusninoc.com/01/06/resolver-el-captcha-de-amazon/
  - Crear e importar dll
    - https://www.jesusninoc.com/11/28/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-c-que-abre-notepad-desde-powershell/
  - Ver qué hace una dll
    - https://www.jesusninoc.com/05/17/funcion-mouse_event-del-archivo-dll-user32-dll/
  - Crear logs
    - https://www.jesusninoc.com/05/04/escribir-y-ver-un-evento-en-el-registro-de-eventos-de-aplicacion/
  - ConvertTo-SecureString
    - https://www.jesusninoc.com/02/19/ejercicios-de-powershell-uso-y-manipulacion-de-credenciales/
  - Colecciones
    - https://www.jesusninoc.com/08/02/2-programacion-en-powershell-nivel-avanzado/
  - Try/catch
    - https://www.jesusninoc.com/02/10/tratamiento-de-excepciones-en-powershell/
  - Objetos
    - https://www.jesusninoc.com/07/02/2-programacion-en-powershell/#Objetos
  - Subir documentos (SharePoint)
    - https://www.jesusninoc.com/12/05/crear-una-conexion-ssh-y-subir-un-fichero-desde-powershell/
  - Sistema de archivos
    - https://www.jesusninoc.com/07/04/4-gestion-del-sistema-de-archivos-en-powershell/

-----------

# 1. Aplicaciones Web

## Introducción
* https://www.jesusninoc.com/11/10/realizar-conexiones-tcp-udp-con-powershell/
* https://www.jesusninoc.com/invoke-webrequest/
* https://www.jesusninoc.com/wget/
* https://www.jesusninoc.com/wordpress/
* https://www.jesusninoc.com/06/07/como-funciona-un-servidor-web-explicado-desde-powershell/
* https://www.jesusninoc.com/06/05/crear-un-servidor-web-con-un-servicio-que-permita-leer-un-codigo-qr-desde-powershell/

## Servidores web
Técnicas de comunicación avanzada. Es una aplicación distribuida basada en el modelo de comunicación cliente/servidor que utiliza el protocolo de nivel de aplicación HTTP para la transferencia de mensajes. Los mensajes se encapsulan dentro de peticiones y respuestas HTTP. Cuando un cliente de un servicio web realiza una petición a un servidor, esta se envía en el interior de un mensaje HTTP, como un GET, POST, o similar. Recordemos que el protocolo HTTP utiliza TCP. Existen varios tipos de servicios web, algunos son: servicios web SOAP y servicios web REST.
* https://www.jesusninoc.com/02/15/crear-un-sitio-en-iis-con-powershell/

## HTTP
### Métodos
* https://www.jesusninoc.com/01/19/metodos-que-se-pueden-utilizar-en-solicitudes-web-en-powershell/
#### GET
* https://www.jesusninoc.com/06/28/temperatura-maxima-en-barcelona-para-hoy/
* https://www.jesusninoc.com/10/12/saber-si-un-nombre-es-de-hombre-o-mujer-con-powershell/
#### GET con valores
* https://www.jesusninoc.com/02/01/get-streets-and-coordinates/
#### Detectar valores GET
* https://www.jesusninoc.com/09/23/detectar-el-formulario-de-busquedas-de-yahoo-y-enviar-una-busqueda-al-formulario/
#### POST
* https://www.jesusninoc.com/04/30/enviar-datos-a-un-formulario-de-google-docs-desde-powershell-deducir-los-parametros-que-se-envian-por-post/
### CRUD
"Crear, Leer, Actualizar y Borrar", que se usa para referirse a las funciones básicas en bases de datos o la capa de persistencia en un software.
### Autenticación
* https://www.jesusninoc.com/02/27/autenticarse-en-un-router-de-fibra-optica-mitrastar-de-movistar-mediante-el-usuario-y-la-contrasena-con-powershell/
### Encabezados
El método HTTP HEAD solicita los encabezados que se devolverían si la URL de la solicitud HEAD se solicitara con el método HTTP GET. Por ejemplo, si una URL puede producir una descarga grande, una solicitud HEAD podría leer su encabezado Content-Length para verificar sin descargar el archivo.
* https://www.jesusninoc.com/07/24/head-method-with-powershell/
* https://www.jesusninoc.com/02/27/autenticarse-en-un-router-de-fibra-optica-mitrastar-de-movistar-mediante-el-usuario-y-la-contrasena-con-powershell/
### Códigos de estado
Cuando Invoke-WebRequest encuentra un mensaje HTTP no exitoso (404, 500, etc.), no devuelve ningún resultado y arroja un error de terminación. Para detectar el error y ver el StatusCode, puede incluir la ejecución en un bloque try/catch.
* https://www.jesusninoc.com/01/30/comprobar-si-un-dominio-responde-y-mostrar-un-mensaje-si-no-responde/
### Codificación
* https://www.jesusninoc.com/07/18/crear-una-web-sencilla-en-chrome-mediante-datos-uris-codificados-en-base64-desde-powershell/
* https://www.jesusninoc.com/03/07/codificar-una-imagen-en-base64-con-powershell/
* https://www.jesusninoc.com/05/05/codificar-un-fichero-bmp-en-base64-con-powershell/
### Token
* https://www.jesusninoc.com/05/04/analizar-la-funcion-autocompletar-de-google-con-fiddler/
* https://www.jesusninoc.com/11/29/apagar-y-encender-la-bombilla-inteligente-tp-link-kasa-regulable-kl110-desde-powershell/
* https://www.jesusninoc.com/02/17/mostrar-el-volumen-diario-de-varias-acciones-del-ibex-35-y-del-mercado-continuo/
* https://www.jesusninoc.com/02/27/enviar-por-mail-el-precio-la-fecha-la-hora-y-el-volumen-de-varias-acciones-del-ibex-35-en-un-momento-concreto/

## WebClient
* https://www.jesusninoc.com/12/09/get-image-for-captcha-session/
* https://www.jesusninoc.com/12/09/read-news-google-news-reproduced-voice-operating-system/

## Invoke-WebRequest
### Propiedades
* https://www.jesusninoc.com/10/07/detectar-si-una-pagina-web-ha-actualizado-el-contenido/
* https://www.jesusninoc.com/03/03/como-conocer-el-tamano-del-resultado-de-una-peticion-web-desde-powershell/
* https://www.jesusninoc.com/02/24/detectar-con-powershell-si-una-camara-emite-en-negro/
### User-Agent
* https://www.jesusninoc.com/07/09/cambiar-el-user-agent/
### Cabeceras
* https://www.jesusninoc.com/01/18/subir-un-video-a-azure-video-indexer/
### Sesiones
* https://www.jesusninoc.com/02/14/almacenar-la-posicion-gps-en-una-variable-de-sesion-en-php/
* https://www.jesusninoc.com/02/26/utilizar-sesiones-de-las-aplicaciones-web-en-powershell/
### Where
* https://www.jesusninoc.com/07/10/html-parsing-get-information-from-a-website-bbc-news-2017/
### Convertir resultado XML
* https://www.jesusninoc.com/02/26/mostrar-las-tendencias-de-busqueda-mas-recientes-en-google-trends/
### Convertir resultado JSON
* https://www.jesusninoc.com/03/08/ver-categorias-de-wordpress-json-api-desde-powershell/
### Problemas SSL
* https://www.jesusninoc.com/02/19/invoke-webrequest-anulada-la-solicitud-no-se-puede-crear-un-canal-seguro-ssl-tls/

## Invoke-RestMethod
* https://www.jesusninoc.com/invoke-restmethod/

## Start-BitsTransfer
* https://www.jesusninoc.com/05/20/descargar-las-imagenes-de-una-pagina-web/

## Ejercicios de PowerShell
- Crear un servidor Web en PowerShell
  - https://www.jesusninoc.com/02/15/crear-un-sitio-en-iis-con-powershell/
- Peticiones con Invoke-WebRequest
- Fiddler y sesiones de las cotizaciones
  - https://www.jesusninoc.com/09/27/arrancar-una-aplicacion-remotamente-desde-powershell-teniendo-habilitado-device-portal/
  - https://www.jesusninoc.com/10/01/listar-el-contenido-de-un-directorio-remotamente-desde-powershell-teniendo-habilitado-device-portal/
  - https://www.jesusninoc.com/06/04/enviar-datos-a-un-formulario-de-google-docs-desde-powershell-pasos-version-04-06-2021/

-----------

# 2. Servicios Web

## Introducción
* https://www.jesusninoc.com/05/17/mostrar-los-precios-de-la-sesion-del-ibex-35-creando-un-servidor-web-al-que-se-pueda-acceder-desde-cualquier-parte-de-la-red-privada-con-powershell/
* https://www.jesusninoc.com/06/05/crear-un-servidor-web-con-un-servicio-que-permita-leer-un-codigo-qr-desde-powershell/
* https://www.jesusninoc.com/02/08/ejercicios-de-php-crear-un-formulario-y-enviar-valores-con-el-metodo-get/
* https://www.jesusninoc.com/05/31/usar-soap-desde-powershell-wsdl/
* https://www.jesusninoc.com/02/01/look-up-countries-by-ip-address/

## SOAP
SOAP es un protocolo estándar que define cómo dos objetos en diferentes procesos pueden comunicarse por medio de intercambio de datos XML. Recibe este nombre debido al formato en que representan los mensajes, sigue el estándar SOAP. En SOAP se utiliza el lenguaje XML para definir tanto el protocolo de mensaje como el contenido de estos. La descripción de interfaz de servicios de un servicio web SOAP se realiza usando un lenguaje basado en XML llamado XDSL.
Un servicio SOAP debe cumplir:
- Expresar de manera formal la interfaz, se suele hacer en WSDL.
- La arquitectura del servicio debe ser capaz de soportar la realización y procesamiento de peticiones de forma asíncrona.

## WSDL
WSDL son las siglas de web service description language o lenguaje de descripción de servicios web. Se trata de un metalenguaje que permite describir los servicios web de manera integral. Un servicio web es, a su vez, un servicio que un servidor proporciona a los clientes a través de Internet (u otra red). Este proceso se lleva a cabo al margen de la plataforma, esto es, entre los sistemas y aplicaciones más diversos. Para que el cliente pueda conocer los procedimientos y posibilidades del servicio web, un archivo WSDL en el servidor web contiene la información que indica al cliente cómo llamar al servicio web.
WSDL se basa en el lenguaje XML (extensible markup language) o lenguaje de marcado extensible, así como en el lenguaje XML Schema (XSD). En otras palabras, WSDL utiliza elementos XML.

## New-WebServiceProxy
* https://www.jesusninoc.com/05/31/usar-soap-desde-powershell-wsdl/

## Ejercicios
- Comprender cómo funciona un servicio web
- Crear un servicio web
  * https://www.jesusninoc.com/02/26/convertir-un-fichero-xml-en-json-desde-php-y-utilizarlo-desde-powershell/ 
- Crear un servicio web en .NET
  * https://www.jesusninoc.com/06/03/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio/
- Crear un servicio Web ASP.NET (ASMX) con Microsoft Visual Studio, publicarlo en un servidor IIS local
  * https://www.jesusninoc.com/06/04/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio-publicarlo-en-un-servidor-iis-local-y-despues-utilizarlo-desde-powershell-con-new-webserviceproxy/
- Crear una aplicación Web en IIS desde PowerShell desarrollada con ASP.NET (ASMX)
  * https://www.jesusninoc.com/06/05/crear-una-aplicacion-web-en-iis-desde-powershell-desarrollada-con-asp-net-asmx-y-despues-utilizar-un-metodo-con-new-webserviceproxy/

## Ejercicios de PowerShell
- Realizar petición tipo POST contra servicio Web online
  * https://www.jesusninoc.com/06/03/realizar-peticion-tipo-post-contra-servicio-web-online/
- Realizar petición tipo POST contra servicio Web
  * https://www.jesusninoc.com/06/03/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio-y-despues-realizar-una-peticion-post-desde-powershell/
- Leer datos de un sercicio Web SOAP online
  * https://www.jesusninoc.com/05/31/usar-soap-desde-powershell-wsdl/
- Leer datos de un servicio Web creado por nosotros
  * https://www.jesusninoc.com/06/03/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio-y-despues-utilizarlo-desde-powershell-con-new-webserviceproxy/

-----------

# 3. REST

## Introducción
REST (Transferencia de Estado Representacional). Define la arquitectura usada en una red, usa como base el protocolo HTTP y nos sirve para generar datos y operaciones devolviendo datos en formato JSON o XML. Puesto que usa HTTP como base, todos los objetos se manipulan a través de una URL. Como alternativa a los servicios basados en SOAP, existe REST. No siguen el estándar SOAP y no están forzados a utilizar XML para representar sus mensajes y su interfaz. Se usa REST, un formato más ligero y flexible.
* https://www.jesusninoc.com/03/08/ver-categorias-de-wordpress-json-api-desde-powershell/

## Definiciones
- Rutas y Puntos finales. Una ruta es una URL que puedes asignar a diferentes métodos HTTP, mientras que un punto final es una conexión entre un método HTTP individual y una ruta. /wp-json/ es un ejemplo de una ruta y contiene todos los puntos finales correspondientes.
- Peticiones. Una instancia de WP_REST_Request. Se utiliza para almacenar y recuperar información para la solicitud actual.
- Respuestas. Proporcionan los datos que solicitaste o devuelven un error que te permite saber qué fue lo que salió mal.
- Esquemas. Muestra una lista de todas las propiedades y parámetros de entrada que la API REST puede aceptar y devolver.
- Clases de controlador. El lugar donde administras las partes móviles de la API REST.

## Ejercicios
- Crear un servicio REST en Visual Studio
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-y-despues-utilizarlo-desde-powershell/
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-anadir-varios-metodos-listar-y-eliminar-y-despues-utilizarlo-desde-powershell/
- Crear un servicio REST con Microsoft Visual Studio, publicarlo en un servidor IIS local
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-anadir-varios-metodos-listar-y-eliminar-publicarlo-en-un-servidor-iis-local-y-despues-llamarlo-desde-powershell/

## Ejercicios de PowerShell
- Llamar a REST en WordPress
  - https://www.jesusninoc.com/03/30/ver-categorias-de-wordpress-json-api-desde-powershell-y-mostrar-el-resultado-en-una-tabla-interactiva/

-----------

# 4. API

## Introducción
Interfaces de programación de aplicaciones. Es una especificación formal de cómo un módulo de software se comunica con otro, es decir, es un conjunto de comandos, funciones y protocolos que permiten a los desarrolladores crear programas específicos para ciertos sistemas sin tener que escribir desde cero todo. Establece un protocolo abstracto de comunicación entre distintas aplicaciones, esto es que no necesite conocer el funcionamiento interno de la aplicación, sino un conjunto de llamadas y la estructura del resultado esperado.
* https://www.jesusninoc.com/webclient/
* https://www.jesusninoc.com/02/26/utilizar-sesiones-de-las-aplicaciones-web-en-powershell/
* https://www.jesusninoc.com/01/25/extraer-informacion-de-sitios-web/
* https://www.jesusninoc.com/start-bitstransfer/
* https://www.jesusninoc.com/02/09/tratamiento-de-errores-en-powershell/
* https://www.jesusninoc.com/01/14/conocer-la-edad-de-una-persona-mediante-el-reconocimiento-optico-de-caracteres-y-el-analisis-de-imagenes-computer-vision-api-de-microsoft-azure/
* https://docs.microsoft.com/es-es/azure/cognitive-services/authentication?tabs=powershell

## Ejercicios de PowerShell
- Llamada al API de algún servicio
  - https://www.jesusninoc.com/03/13/exportar-e-importar-un-objeto-json-que-se-encuentra-en-una-web-desde-powershell/
  - https://www.jesusninoc.com/rutinas2.html
  - https://www.jesusninoc.com/02/07/falcon-heavy-spacex-data-rest-api/
  - https://www.jesusninoc.com/01/14/ejercicios-de-powershell-crear-usuarios-con-nombres-aleatorios-utilizando-un-api-que-devuelve-el-resultado-en-formato-json/