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

## Funcionamiento
* https://docs.microsoft.com/es-es/aspnet/core/tutorials/first-web-api/_static/architecture.png?view=aspnetcore-5.0

## RESTful API
RESTful API es el sucesor de métodos anteriores como SOAP y WSDL cuya implementación y uso son un poco mas complejos y requieren mayores recursos y especificaciones al ser usados.

## Principios rectores de REST
- Cliente-servidor : al separar las preocupaciones de la interfaz de usuario de las preocupaciones de almacenamiento de datos, mejoramos la portabilidad de la interfaz de usuario en múltiples plataformas y mejoramos la escalabilidad al simplificar los componentes del servidor.
- Sin estado : cada solicitud del cliente al servidor debe contener toda la información necesaria para comprender la solicitud y no puede aprovechar ningún contexto almacenado en el servidor. Por lo tanto, el estado de la sesión se mantiene completamente en el cliente.
- Se puede almacenar en caché: las restricciones de caché requieren que los datos dentro de una respuesta a una solicitud se etiqueten implícita o explícitamente como almacenables en caché o no almacenables en caché. Si una respuesta se puede almacenar en caché, la caché de un cliente tiene derecho a reutilizar esos datos de respuesta para solicitudes posteriores equivalentes.
- Interfaz uniforme : al aplicar el principio de generalidad de la ingeniería de software a la interfaz del componente, se simplifica la arquitectura general del sistema y se mejora la visibilidad de las interacciones. Para obtener una interfaz uniforme, se necesitan múltiples restricciones arquitectónicas para guiar el comportamiento de los componentes. REST se define por cuatro restricciones de interfaz: identificación de recursos; manipulación de recursos a través de representaciones; mensajes autodescriptivos; e hipermedia como motor del estado de la aplicación.
- Sistema en capas: el estilo de sistema en capas permite que una arquitectura se componga de capas jerárquicas al restringir el comportamiento de los componentes de manera que cada componente no pueda "ver" más allá de la capa inmediata con la que están interactuando.
- Código a pedido (opcional) : REST permite ampliar la funcionalidad del cliente descargando y ejecutando código en forma de subprogramas o scripts. Esto simplifica a los clientes al reducir la cantidad de funciones que deben implementarse previamente.

## Ejercicios
- Crear un servicio REST API en Visual Studio
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-y-despues-utilizarlo-desde-powershell/
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-anadir-varios-metodos-listar-y-eliminar-y-despues-utilizarlo-desde-powershell/
- Crear un servicio REST API con Microsoft Visual Studio, publicarlo en un servidor IIS local
  - https://www.jesusninoc.com/06/06/crear-un-servicio-web-asp-net-web-api-rest-con-microsoft-visual-studio-anadir-varios-metodos-listar-y-eliminar-publicarlo-en-un-servidor-iis-local-y-despues-llamarlo-desde-powershell/

## Ejercicios de PowerShell
- Llamada al API de algún servicio
  - https://www.jesusninoc.com/03/13/exportar-e-importar-un-objeto-json-que-se-encuentra-en-una-web-desde-powershell/
  - https://www.jesusninoc.com/rutinas2.html
  - https://api.spacexdata.com/v2/
  - https://www.jesusninoc.com/02/07/falcon-heavy-spacex-data-rest-api/
  - https://www.jesusninoc.com/01/14/ejercicios-de-powershell-crear-usuarios-con-nombres-aleatorios-utilizando-un-api-que-devuelve-el-resultado-en-formato-json/
