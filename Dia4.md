# Repaso temario

## DocuWare
* https://developer.docuware.com/
* https://developer.docuware.com/dotNet/66b2ed1e-2aef-452a-97cd-5014bbf0242b.html
* https://docs.microsoft.com/es-es/nuget/consume-packages/install-use-packages-visual-studio
* https://developer.docuware.com/dotNet_CodeExamples/8ecbfe35-9182-4acc-833e-ac0f1857347e.html
```PowerShell
[Reflection.Assembly]::LoadFile("C:\Users\juan\.nuget\packages\docuware.platform.serverclient\12.2.1\lib\net472\DocuWare.Platform.ServerClient.dll")
[Reflection.Assembly]::LoadFile("C:\Users\juan\.nuget\packages\docuware.restclient\10.4.300696\lib\net472\DocuWare.RestClient.dll")
[Reflection.Assembly]::LoadFile("C:\Users\juan\.nuget\packages\docuware.uritemplates\10.5.358704\lib\net472\DocuWare.UriTemplates.dll")
```
## Sesiones
* https://www.jesusninoc.com/02/26/utilizar-sesiones-de-las-aplicaciones-web-en-powershell/#Codigo_en_PHP_que_cierra_una_sesion_iniciada_anteriormente_tercerophp
* https://www.jesusninoc.com/06/23/utilizar-sesiones-web-en-powershell-desde-un-powershell-crear-una-sesion-almacenarla-en-un-fichero-y-despues-abrir-otro-powershell-e-importar-la-sesion-guardada/
## Cookies
* https://www.jesusninoc.com/06/09/autenticarse-en-el-punto-de-acceso-mediante-el-usuario-y-la-contrasena-autorizacion-authorization-de-tipo-basic-enviada-por-cookie/
## Llamar a un servicio Web
* https://www.jesusninoc.com/06/23/diferentes-formas-de-llamar-a-un-servicio-web-desde-powershell/

-----------------

# 3. API

## Introducción
Interfaces de programación de aplicaciones. Es una especificación formal de cómo un módulo de software se comunica con otro, es decir, es un conjunto de comandos, funciones y protocolos que permiten a los desarrolladores crear programas específicos para ciertos sistemas sin tener que escribir desde cero todo. Establece un protocolo abstracto de comunicación entre distintas aplicaciones, esto es que no necesite conocer el funcionamiento interno de la aplicación, sino un conjunto de llamadas y la estructura del resultado esperado.

La diferencia principal es que el servicio Web facilita que dos máquinas interactúen a través de una red, mientras que una API es una interfaz. Y a través de ella dos aplicaciones establecen comunicación.
* https://www.jesusninoc.com/webclient/
* https://www.jesusninoc.com/02/26/utilizar-sesiones-de-las-aplicaciones-web-en-powershell/
* https://www.jesusninoc.com/01/25/extraer-informacion-de-sitios-web/
* https://www.jesusninoc.com/start-bitstransfer/
* https://www.jesusninoc.com/02/09/tratamiento-de-errores-en-powershell/
* https://www.jesusninoc.com/01/14/conocer-la-edad-de-una-persona-mediante-el-reconocimiento-optico-de-caracteres-y-el-analisis-de-imagenes-computer-vision-api-de-microsoft-azure/
* https://docs.microsoft.com/es-es/azure/cognitive-services/authentication?tabs=powershell

## Situación inicial: crear un sistema que permita devolver información en formato JSON sobre un coche (http://localhost/coche)
* https://www.jesusninoc.com/06/24/crear-un-sistema-en-powershell-que-permita-devolver-informacion-en-formato-json-sobre-un-coche/

## Funcionamiento web API
* https://docs.microsoft.com/es-es/aspnet/core/tutorials/first-web-api/_static/architecture.png?view=aspnetcore-5.0

## ¿Que es REST o RESTful como WebService?
REST se define como Transferencia de estado representacional en inglés (REpresentational State Transfer).

REST no define tantos estándares como SOAP. REST es para exponer las API públicas (es decir, la API de Facebook, la API de Google Maps) a través de Internet para manejar las operaciones de CRUD en los datos. REST se enfoca en acceder a recursos nombrados a través de una única interfaz consistente.

RESTful hace referencia a un servicio web que implementa la arquitectura REST.

## RESTful API
RESTful API es el sucesor de métodos anteriores como SOAP y WSDL cuya implementación y uso son un poco mas complejos y requieren mayores recursos y especificaciones al ser usados.

## Se considera que una aplicación es RESTful si cumple con seis pautas arquitectónicas. Una aplicación de RESTful debe tener lo siguiente:
- Una arquitectura cliente-servidor compuesta por clientes, servidores y recursos.
- Una comunicación cliente-servidor sin estado, lo cual significa que el contenido de los clientes no se almacena en el servidor entre las solicitudes, sino que la información sobre el estado de la sesión queda en el cliente.
- Datos que pueden almacenarse en caché para eliminar la necesidad de algunas interacciones cliente-servidor.
- Una interfaz uniforme entre elementos para que la información se transfiera de forma estandarizada, en lugar de ser específica para las necesidades de cierta aplicación. Roy Fielding, el creador de REST, lo describe como "la característica principal que distingue el estilo arquitectónico de REST de los demás estilos basados en la red".
- Una restricción del sistema en capas, en el que las interacciones cliente-servidor pueden estar mediadas por capas jerárquicas.
Código según se solicite, lo que permite que los servidores amplíen las funciones de un cliente al transferir el código ejecutable (esto también reduce la visibilidad, así que es una pauta opcional).

#### Ejercicios
- Crear un servicio REST API en Visual Studio
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-y-despues-utilizarlo-desde-powershell/
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-anadir-varios-metodos-listar-y-eliminar-y-despues-utilizarlo-desde-powershell/
- Crear un servicio REST API con Microsoft Visual Studio, publicarlo en un servidor IIS local
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-anadir-varios-metodos-listar-y-eliminar-publicarlo-en-un-servidor-iis-local-y-despues-llamarlo-desde-powershell/

#### Ejercicios de PowerShell
- Llamada al API de algún servicio
  - https://www.jesusninoc.com/03/13/exportar-e-importar-un-objeto-json-que-se-encuentra-en-una-web-desde-powershell/
  - https://www.jesusninoc.com/rutinas2.html
  - https://api.spacexdata.com/v2/
  - https://www.jesusninoc.com/02/07/falcon-heavy-spacex-data-rest-api/
  - https://www.jesusninoc.com/01/14/ejercicios-de-powershell-crear-usuarios-con-nombres-aleatorios-utilizando-un-api-que-devuelve-el-resultado-en-formato-json/

## GraphQL
* https://www.jesusninoc.com/06/01/realizar-una-peticion-graphql-desde-powershell/
