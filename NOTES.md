# INSTALACIÓN

1. dotnet new webapi -controllers

# Middlewares:

- Es una serie de instrucciones de código que se agregan al cilco de vida de una petición HTTP.

Provee una ejecucion de peticiones a través de capas.

Facilitan la implementación de interceptores y filtros sobre las peticiones en una API.

# Middleware personalizado:

1. En raiz crear una carpeta llamada middlewares
2. Dentro crear un archivo llamado TimeMiddleware.cs

# Inyección de dependencias

1. Crear una carpeta en raiz llamada Services
2. Crear un archivo dentro llamado HelloWordServices.cs

# Agregando Logs a API

1. En este caso se pasó en los controladores, ver ejemplo en weatherforescastController
2. En appsettings.development.json: en el loglevel especificar que nivel de log quiero, buscar la documentacion para ver los logs: logging dotnet core

# Documentando API con Swagger

1. Usa el standard OpenApi
2. Se corre el proyect dotnet run
3. Ir al localhost que da la consola y agregarle /swagger y saldrá la documentación
4. Solo se implementa en ambiente de desarrollo.

# Agregando librerías para Entity Framework:

1. Ir a nuget.org y buscar Microsoft.EntityFrameworkCore y seleccionar la ultima versión estable, copiar el codigo y pegarlo en la consola.
2. Ir a nuget.org y buscar Microsoft.EntityFrameworkCore.InMemory seleccionar la ultima versión estable, copiar el codigo y pegarlo en la consola
3. Ir a nuget.org y buscar Microsoft.EntityFrameworkCore.SqlServer seleccionar la ultima versión estable, copiar el codigo y pegarlo en la consola

# Configuración de Entity framework y clases base

1. Copiar en raiz el archivo TareasContext.cs y la carpeta models del proyecto de EntityFramework

# Creación de servicios

1. Se creará un servicio para cada modelo
2. Crear una carpeta llamada Services y dentro un archivo llamado CategoriaService.cs y colocar la logica para el service
3. Dentro de Services crear un archivo llamado TareasService.cs y colocar la logica

# Inyectando servicios como dependencia

1.  En program.cs

# Crear los controladores.

1. Dentro de la carpeta Controllers crear CategoriaController.cs y TareaController.cs

# Probando API con una base de datos SQL server

1. En program.cs configurar entity framework
