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

## Ejercicios
- Comprender cómo funciona un servicio web. En la arquitectura de servicios web existen tres partes: proveedor de servicios web, el que pide el servicio web y el publicador. El proveedor de servicios envía al publicador del servicio un fichero WSDL con la definición del servicio web. El que pide el servicio contacta con el publicador y descubre quién es el proveedor (protocolo WSDL) y contacta con el proveedor (protocolo SOAP). El proveedor valida la petición de servicio y envía el dato estructurado en formato XML utilizando el protocolo SOAP. El fichero XML es validado de nuevo por el que pide el servicio utilizando un fichero XSD.
  * https://es.wikipedia.org/wiki/Servicio_web#/media/Archivo:Webservices-en.svg
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

## Ejercicios de PowerShell
- Llamar a REST en WordPress
  - https://www.jesusninoc.com/03/30/ver-categorias-de-wordpress-json-api-desde-powershell-y-mostrar-el-resultado-en-una-tabla-interactiva/
