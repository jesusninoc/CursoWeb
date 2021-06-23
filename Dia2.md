# 0. Presentación
- Conceptos que he visto en los scripts pero que no son web:
  - Crear e importar dll
    - https://www.jesusninoc.com/06/08/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-studio-c-y-utilizarla-desde-powershell/
    - https://www.jesusninoc.com/11/28/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-c-que-abre-notepad-desde-powershell/
  - Try/catch (una excepción es cualquier evento que ocurre durante la ejecución de un programa que interrumpe el flujo normal de ejecución
    - https://www.jesusninoc.com/02/10/tratamiento-de-excepciones-en-powershell/
  - Objetos
    - https://www.jesusninoc.com/07/02/2-programacion-en-powershell/#Objetos
  - Subir documentos (SharePoint)
    - https://www.jesusninoc.com/12/05/crear-una-conexion-ssh-y-subir-un-fichero-desde-powershell/
  - Sistema de archivos
    - https://www.jesusninoc.com/07/04/4-gestion-del-sistema-de-archivos-en-powershell/

-----------

# 1. Aplicaciones Web
Aplicaciones Web y servicios (la diferencia entre una aplicación web y un servicio web es que la aplicación web es un sistema de gestión diseñado para ser usado por humanos, mientras que un servicio web es un sistema diseñado para ser usado por otras aplicaciones o sistemas).

## Introducción
* https://www.jesusninoc.com/10/07/crear-un-cliente-y-un-servidor-tcpip-con-powershell/
* https://www.jesusninoc.com/06/22/crear-un-cliente-y-un-servidor-tcp-ip-que-recibe-una-sola-peticion-con-powershell-hacerlo-de-forma-simple/
* https://www.jesusninoc.com/11/10/realizar-conexiones-tcp-udp-con-powershell/
* https://www.jesusninoc.com/invoke-webrequest/
* https://www.jesusninoc.com/wget/
* https://www.jesusninoc.com/wordpress/

## Servidores web
* https://www.jesusninoc.com/06/07/como-funciona-un-servidor-web-explicado-desde-powershell/
* https://www.jesusninoc.com/06/05/crear-un-servidor-web-con-un-servicio-que-permita-leer-un-codigo-qr-desde-powershell/

#### Ejercicios de PowerShell
- Crear un sitio web
  - https://www.jesusninoc.com/02/15/crear-un-sitio-en-iis-con-powershell/
- Crear varios sitios web para varios clientes cuyos nombres están en un fichero
  - https://www.jesusninoc.com/06/22/ejercicios-de-powershell-crear-varios-sitios-web-para-varios-clientes-cuyos-nombres-estan-en-un-fichero/ 

## HTTP
### Métodos
* https://www.jesusninoc.com/01/19/metodos-que-se-pueden-utilizar-en-solicitudes-web-en-powershell/
#### GET
* https://www.jesusninoc.com/06/28/temperatura-maxima-en-barcelona-para-hoy/
#### GET con valores
* https://www.jesusninoc.com/02/01/get-streets-and-coordinates/
* https://www.jesusninoc.com/06/20/detectar-el-formulario-de-busquedas-de-una-pagina-web-y-enviar-una-busqueda-al-formulario-desde-powershell-con-webclient-system-net-webclient/
#### Detectar valores GET
* https://www.jesusninoc.com/09/23/detectar-el-formulario-de-busquedas-de-yahoo-y-enviar-una-busqueda-al-formulario/
#### POST
* https://www.jesusninoc.com/04/30/enviar-datos-a-un-formulario-de-google-docs-desde-powershell-deducir-los-parametros-que-se-envian-por-post/
### CRUD
"Crear, Leer, Actualizar y Borrar", que se usa para referirse a las funciones básicas en bases de datos o la capa de persistencia en un software.
### Encabezados
Las Cabeceras HTTP son los parámetros que se envían en una petición o respuesta HTTP al cliente o al servidor para proporcionar información esencial sobre la transacción encurso. Estas cabeceras proporcionan información mediante la sintaxis 'Cabecera:Valor' y son enviadas automáticamente por el navegador o el servidor Web. El método HTTP HEAD solicita los encabezados que se devolverían si la URL de la solicitud HEAD se solicitara con el método HTTP GET. Por ejemplo, si una URL puede producir una descarga grande, una solicitud HEAD podría leer su encabezado Content-Length para verificar sin descargar el archivo.
* https://www.jesusninoc.com/07/24/head-method-with-powershell/
* https://www.jesusninoc.com/12/15/ver-la-tabla-de-direcciones-mac-asociadas-a-un-punto-de-acceso/
* https://www.jesusninoc.com/01/14/conocer-la-edad-de-una-persona-mediante-el-reconocimiento-optico-de-caracteres-y-el-analisis-de-imagenes-computer-vision-api-de-microsoft-azure/
* https://www.jesusninoc.com/02/27/autenticarse-en-un-router-de-fibra-optica-mitrastar-de-movistar-mediante-el-usuario-y-la-contrasena-con-powershell/
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
Un token de sesión es un identificador único que está generado y enviado desde un servidor a un cliente para identificar la sesión de interacción actual. El cliente envía el token como una cookie HTTP y/o lo envía como parámetro en GET o POST. La razón para utilizar tokens de sesión es que el cliente sólo tiene que manejar el identificador—toda la información de sesión está almacenada en el servidor (normalmente en una base de datos, al cual el cliente no tiene acceso directo) enlazada a aquel identificador. Ejemplos de los nombres que algunos lenguajes de programación utilizan cuándo se nombra su cookie HTTP son: JSESSIONID (JSP),PHPSESSID (PHP), CGISESSID (CGI), y ASPSESSIONID (ASP).
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
