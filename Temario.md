
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
