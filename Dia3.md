# 1. Aplicaciones Web
Aplicaciones Web y servicios (la diferencia entre una aplicación web y un servicio web es que la aplicación web es un sistema de gestión diseñado para ser usado por humanos, mientras que un servicio web es un sistema diseñado para ser usado por otras aplicaciones o sistemas).

## HTTP
### Códigos de estado
Cuando Invoke-WebRequest encuentra un mensaje HTTP no exitoso (404, 500, etc.), no devuelve ningún resultado y arroja un error de terminación. Para detectar el error y ver el StatusCode, puede incluir la ejecución en un bloque try/catch.
* https://www.jesusninoc.com/01/30/comprobar-si-un-dominio-responde-y-mostrar-un-mensaje-si-no-responde/
### Codificación
Los mensajes HTTP, son los medios por los cuales se intercambian datos entre servidores y clientes. Hay dos tipos de mensajes: peticiones, enviadas por el cliente al servidor, para pedir el inicio de una acción; y respuestas, que son la respuesta del servidor. 
Los mensajes HTTP están compuestos de texto, codificado en ASCII, y pueden comprender múltiples líneas. En HTTP/1.1, y versiones previas del protocolo, estos mensajes eran enviados de forma abierta a través de la conexión. En HTTP/2.0 los mensajes, que anteriormente eran legibles directamente, se conforman mediante tramas binarias codificadas para aumentar la optimización y rendimiento de la transmisión.
Los desarrolladores de páginas Web, o administradores de sitios Web, desarrolladores... raramente codifican directamente estos mensajes HTTP. Normalmente especifican estos mensajes HTTP, mediante archivos de configuración (para proxies, y servidores), APIs (para navegadores) y otros medios.
* https://www.jesusninoc.com/07/18/crear-una-web-sencilla-en-chrome-mediante-datos-uris-codificados-en-base64-desde-powershell/
* https://www.jesusninoc.com/03/07/codificar-una-imagen-en-base64-con-powershell/
* https://www.jesusninoc.com/05/05/codificar-un-fichero-bmp-en-base64-con-powershell/
### Autenticación
* https://www.jesusninoc.com/02/27/autenticarse-en-un-router-de-fibra-optica-mitrastar-de-movistar-mediante-el-usuario-y-la-contrasena-con-powershell/
* https://www.jesusninoc.com/01/14/conocer-la-edad-de-una-persona-mediante-el-reconocimiento-optico-de-caracteres-y-el-analisis-de-imagenes-computer-vision-api-de-microsoft-azure/
### Cookies
* https://www.jesusninoc.com/06/09/autenticarse-en-el-punto-de-acceso-mediante-el-usuario-y-la-contrasena-autorizacion-authorization-de-tipo-basic-enviada-por-cookie/
* https://www.jesusninoc.com/02/26/utilizar-sesiones-de-las-aplicaciones-web-en-powershell/
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
Invoke-RestMethod es básicamente un cmdlet contenedor entorno a Invoke-WebRequest. Invoke-RestMethod realiza una conversión automática. Si la API que está consumiendo devuelve JSON, Invoke-RestMethod devolverá un objeto PowerShell que es el resultado de la conversión JSON.
Invoke-RestMethod es mucho mejor para tratar con resultados XML y JSON, mientras que Invoke-WebRequest es mejor para tratar con resultados HTML directos.
* https://www.jesusninoc.com/invoke-restmethod/

## Start-BitsTransfer
* https://www.jesusninoc.com/05/20/descargar-las-imagenes-de-una-pagina-web/

#### Ejercicios
- Crear un servicio web en .NET
  * https://www.jesusninoc.com/06/03/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio/
- Crear un servicio Web ASP.NET (ASMX) con Microsoft Visual Studio, publicarlo en un servidor IIS local
  * https://www.jesusninoc.com/06/04/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio-publicarlo-en-un-servidor-iis-local-y-despues-utilizarlo-desde-powershell-con-new-webserviceproxy/

#### Ejercicios de PowerShell
- Peticiones con Invoke-WebRequest, Invoke-RestMethod y Start-BitsTransfer
- Fiddler y sesiones de las cotizaciones
  - https://www.jesusninoc.com/09/27/arrancar-una-aplicacion-remotamente-desde-powershell-teniendo-habilitado-device-portal/
  - https://www.jesusninoc.com/10/01/listar-el-contenido-de-un-directorio-remotamente-desde-powershell-teniendo-habilitado-device-portal/
  - https://www.jesusninoc.com/06/04/enviar-datos-a-un-formulario-de-google-docs-desde-powershell-pasos-version-04-06-2021/

-------------------

# 2. Servicios Web

## Introducción
Técnicas de comunicación avanzada. Es una aplicación distribuida basada en el modelo de comunicación cliente/servidor que utiliza el protocolo de nivel de aplicación HTTP para la transferencia de mensajes. Los mensajes se encapsulan dentro de peticiones y respuestas HTTP. Cuando un cliente de un servicio web realiza una petición a un servidor, esta se envía en el interior de un mensaje HTTP, como un GET, POST, o similar. Recordemos que el protocolo HTTP utiliza TCP. Existen varios tipos de servicios web, algunos son: servicios web SOAP y servicios web REST.

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

### WSDL
WSDL son las siglas de web service description language o lenguaje de descripción de servicios web. Se trata de un metalenguaje que permite describir los servicios web de manera integral. Un servicio web es, a su vez, un servicio que un servidor proporciona a los clientes a través de Internet (u otra red). Este proceso se lleva a cabo al margen de la plataforma, esto es, entre los sistemas y aplicaciones más diversos. Para que el cliente pueda conocer los procedimientos y posibilidades del servicio web, un archivo WSDL en el servidor web contiene la información que indica al cliente cómo llamar al servicio web.
WSDL se basa en el lenguaje XML (extensible markup language) o lenguaje de marcado extensible, así como en el lenguaje XML Schema (XSD). En otras palabras, WSDL utiliza elementos XML.

## New-WebServiceProxy
Los clientes invocan a los métodos de los prosees como si estuvieran implementados en local.
* https://www.jesusninoc.com/05/31/usar-soap-desde-powershell-wsdl/

### Ejercicios
- Comprender cómo funciona un servicio web. En la arquitectura de servicios web existen tres partes: proveedor de servicios web, el que pide el servicio web y el publicador. El proveedor de servicios envía al publicador del servicio un fichero WSDL con la definición del servicio web. El que pide el servicio contacta con el publicador y descubre quién es el proveedor (fichero WSDL) y contacta con el proveedor (protocolo SOAP). El proveedor valida la petición de servicio y envía el dato estructurado en formato XML utilizando el protocolo SOAP. El fichero XML es validado de nuevo por el que pide el servicio utilizando un fichero XSD.
  * https://es.wikipedia.org/wiki/Servicio_web#/media/Archivo:Webservices-en.svg
- Crear un servicio web
  * https://www.jesusninoc.com/02/26/convertir-un-fichero-xml-en-json-desde-php-y-utilizarlo-desde-powershell/ 
- Crear un servicio web en .NET
  * https://www.jesusninoc.com/06/03/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio/
- Crear un servicio Web ASP.NET (ASMX) con Microsoft Visual Studio, publicarlo en un servidor IIS local
  * https://www.jesusninoc.com/06/04/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio-publicarlo-en-un-servidor-iis-local-y-despues-utilizarlo-desde-powershell-con-new-webserviceproxy/
- Crear una aplicación Web en IIS desde PowerShell desarrollada con ASP.NET (ASMX)
  * https://www.jesusninoc.com/06/05/crear-una-aplicacion-web-en-iis-desde-powershell-desarrollada-con-asp-net-asmx-y-despues-utilizar-un-metodo-con-new-webserviceproxy/

### Ejercicios de PowerShell
- Realizar petición tipo POST contra servicio Web online
  * https://www.jesusninoc.com/06/03/realizar-peticion-tipo-post-contra-servicio-web-online/
- Realizar petición tipo POST contra servicio Web
  * https://www.jesusninoc.com/06/03/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio-y-despues-realizar-una-peticion-post-desde-powershell/
- Leer datos de un sercicio Web SOAP online
  * https://www.jesusninoc.com/05/31/usar-soap-desde-powershell-wsdl/
- Leer datos de un servicio Web creado por nosotros
  * https://www.jesusninoc.com/06/03/crear-un-servicio-web-asp-net-asmx-con-microsoft-visual-studio-y-despues-utilizarlo-desde-powershell-con-new-webserviceproxy/

----------------

## REST
REST (Transferencia de Estado Representacional). Define la arquitectura usada en una red, usa como base el protocolo HTTP y nos sirve para generar datos y operaciones devolviendo datos en formato JSON o XML. Puesto que usa HTTP como base, todos los objetos se manipulan a través de una URL. Como alternativa a los servicios basados en SOAP, existe REST. No siguen el estándar SOAP y no están forzados a utilizar XML para representar sus mensajes y su interfaz. Se usa REST, un formato más ligero y flexible.
* https://www.jesusninoc.com/03/08/ver-categorias-de-wordpress-json-api-desde-powershell/

### Definiciones
- Rutas y Puntos finales. Una ruta es una URL que puedes asignar a diferentes métodos HTTP, mientras que un punto final es una conexión entre un método HTTP individual y una ruta. /wp-json/ es un ejemplo de una ruta y contiene todos los puntos finales correspondientes.
- Peticiones. Una instancia de WP_REST_Request. Se utiliza para almacenar y recuperar información para la solicitud actual.
- Respuestas. Proporcionan los datos que solicitaste o devuelven un error que te permite saber qué fue lo que salió mal.
- Esquemas. Muestra una lista de todas las propiedades y parámetros de entrada que la API REST puede aceptar y devolver.
- Clases de controlador. El lugar donde administras las partes móviles de la API REST.

#### Ejercicios de PowerShell
- Llamar a REST en WordPress
  - https://www.jesusninoc.com/03/30/ver-categorias-de-wordpress-json-api-desde-powershell-y-mostrar-el-resultado-en-una-tabla-interactiva/
