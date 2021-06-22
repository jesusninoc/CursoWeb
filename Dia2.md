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
 ```PowerShell
 Import-Module webadministration

Set-Location IIS:\AppPools\

$numero = 81

foreach($valor in Get-Content C:\Users\juan\clientes.txt)
{
    $web = New-Item C:\web\$valor –ItemType directory -Force
    "<html>hola "+$Valor+"</html>" | Out-File C:\web\$valor\index.html
    $Website = New-Website -Name $valor -HostHeader "" -Port $numero -PhysicalPath $web -ApplicationPool "DefaultAppPool"
    $numero = $numero + 1
}
 ```

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
Las Cabeceras HTTP son los parámetros que se envían en una petición o respuesta HTTP al cliente oal servidor para proporcionar información esencial sobre la transacción encurso. Estas cabeceras proporcionan información mediante la sintaxis 'Cabecera:Valor' y son enviadas automáticamente por el navegador o el servidor Web. El método HTTP HEAD solicita los encabezados que se devolverían si la URL de la solicitud HEAD se solicitara con el método HTTP GET. Por ejemplo, si una URL puede producir una descarga grande, una solicitud HEAD podría leer su encabezado Content-Length para verificar sin descargar el archivo.
* https://www.jesusninoc.com/07/24/head-method-with-powershell/
* https://www.jesusninoc.com/12/15/ver-la-tabla-de-direcciones-mac-asociadas-a-un-punto-de-acceso/
* https://www.jesusninoc.com/01/14/conocer-la-edad-de-una-persona-mediante-el-reconocimiento-optico-de-caracteres-y-el-analisis-de-imagenes-computer-vision-api-de-microsoft-azure/
* https://www.jesusninoc.com/02/27/autenticarse-en-un-router-de-fibra-optica-mitrastar-de-movistar-mediante-el-usuario-y-la-contrasena-con-powershell/
