# 0. Presentación
- Tres horas por tema (introducción, configuraciones, ejercicios resueltos por mi, tiempo para hacer ejercicios)
- Aplicaciones Web
- Servicios
- Otros conceptos que he visto en los scripts pero que no son web:
  - OCR (bucle y ver palabras mal escritas)
    - https://www.jesusninoc.com/01/06/resolver-el-captcha-de-amazon/
    - https://www.jesusninoc.com/02/09/aclarar-una-imagen-utilizando-imagemagick-y-convertir-a-texto-con-tesseract/
    - https://www.jesusninoc.com/02/08/aclarar-una-imagen-utilizando-imagemagick-quitando-ruido-de-una-imagen/
    - https://www.jesusninoc.com/06/11/detectar-las-palabras-que-estan-mal-escritas-en-un-texto-con-un-comando-en-linux-y-ejecutarlo-con-wsl-windows-subsystem-for-linux-desde-powershell/
  - Crear e importar dll
    - https://www.jesusninoc.com/06/08/crear-compilar-y-ejecutar-una-dll-con-microsoft-visual-studio-c-y-utilizarla-desde-powershell/
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
* https://www.jesusninoc.com/10/07/crear-un-cliente-y-un-servidor-tcpip-con-powershell/
* https://www.jesusninoc.com/11/10/realizar-conexiones-tcp-udp-con-powershell/
* https://www.jesusninoc.com/invoke-webrequest/
* https://www.jesusninoc.com/wget/
* https://www.jesusninoc.com/wordpress/

## Servidores web
* https://www.jesusninoc.com/06/07/como-funciona-un-servidor-web-explicado-desde-powershell/
* https://www.jesusninoc.com/06/05/crear-un-servidor-web-con-un-servicio-que-permita-leer-un-codigo-qr-desde-powershell/
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
### Encabezados
El método HTTP HEAD solicita los encabezados que se devolverían si la URL de la solicitud HEAD se solicitara con el método HTTP GET. Por ejemplo, si una URL puede producir una descarga grande, una solicitud HEAD podría leer su encabezado Content-Length para verificar sin descargar el archivo.
* https://www.jesusninoc.com/07/24/head-method-with-powershell/
* https://www.jesusninoc.com/12/15/ver-la-tabla-de-direcciones-mac-asociadas-a-un-punto-de-acceso/
* https://www.jesusninoc.com/01/14/conocer-la-edad-de-una-persona-mediante-el-reconocimiento-optico-de-caracteres-y-el-analisis-de-imagenes-computer-vision-api-de-microsoft-azure/
* https://www.jesusninoc.com/02/27/autenticarse-en-un-router-de-fibra-optica-mitrastar-de-movistar-mediante-el-usuario-y-la-contrasena-con-powershell/
### Códigos de estado
Cuando Invoke-WebRequest encuentra un mensaje HTTP no exitoso (404, 500, etc.), no devuelve ningún resultado y arroja un error de terminación. Para detectar el error y ver el StatusCode, puede incluir la ejecución en un bloque try/catch.
* https://www.jesusninoc.com/01/30/comprobar-si-un-dominio-responde-y-mostrar-un-mensaje-si-no-responde/
### Codificación
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

## Ejercicios de PowerShell
- Leer varios ficheros y pasar OCR
- Crear un servidor Web en PowerShell
  - https://www.jesusninoc.com/02/15/crear-un-sitio-en-iis-con-powershell/
- Peticiones con Invoke-WebRequest
- Fiddler y sesiones de las cotizaciones
  - https://www.jesusninoc.com/09/27/arrancar-una-aplicacion-remotamente-desde-powershell-teniendo-habilitado-device-portal/
  - https://www.jesusninoc.com/10/01/listar-el-contenido-de-un-directorio-remotamente-desde-powershell-teniendo-habilitado-device-portal/
  - https://www.jesusninoc.com/06/04/enviar-datos-a-un-formulario-de-google-docs-desde-powershell-pasos-version-04-06-2021/

## Ejercicios de PowerShell (propuestos)
- Instalar Visual Studio
