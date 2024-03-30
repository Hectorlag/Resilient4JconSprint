Proyecto de Servicios de Java con Eureka Server y OpenFeign
Este proyecto consiste en un sistema distribuido desarrollado en Java que utiliza Eureka Server para el registro y descubrimiento de servicios, junto con OpenFeign para la comunicación entre los servicios. El objetivo principal es simular un sistema de gestión de hoteles y ciudades, donde los servicios de hoteles consumen información de los servicios de ciudades para proporcionar funcionalidades como búsqueda y reservas.

Estructura del Proyecto
El proyecto está organizado en tres carpetas principales:

Eureka Server: Esta carpeta contiene el servidor Eureka, que se encarga de actuar como registro centralizado para todos los servicios en la arquitectura. Permite a los servicios registrarse y descubrirse entre sí de manera dinámica.

Service Hotel: Este servicio representa la funcionalidad relacionada con los hoteles. Actúa como un cliente de descubrimiento de servicios, utilizando OpenFeign para comunicarse con el servicio de ciudades y obtener información relevante para la gestión de hoteles.

Service Cities: Este servicio proporciona información relacionada con las ciudades. También actúa como un cliente de descubrimiento de servicios, permitiendo a otros servicios, como el de hoteles, consumir su funcionalidad a través de OpenFeign.

Tecnologías Utilizadas
Java: El lenguaje principal de programación utilizado en todo el proyecto.
Spring Boot: Utilizado para la creación de aplicaciones Java basadas en Spring de manera rápida y sencilla.
Eureka Server: Herramienta de registro y descubrimiento de servicios desarrollada por Netflix.
OpenFeign: Cliente HTTP declarativo para servicios web. Se utiliza para simplificar las llamadas a los servicios RESTful.
Base de Datos: Utilicé una base de datos lógica para almacenar información.
Configuración y Uso
Eureka Server:

Accede a la carpeta eureka-server.
Ejecuta la aplicación Spring Boot para iniciar el servidor Eureka.
El servidor Eureka estará disponible en la dirección predeterminada http://localhost:8761.
Service Hotel:

Accede a la carpeta service-hotel.
Configura las propiedades de conexión a Eureka Server en el archivo application.properties.
Ejecuta la aplicación Spring Boot para iniciar el servicio de hoteles.
Service Cities:

Accede a la carpeta service-cities.
Configura las propiedades de conexión a Eureka Server en el archivo application.properties.
Ejecuta la aplicación Spring Boot para iniciar el servicio de ciudades.
Colaboración
Si deseas contribuir a este proyecto, ¡te damos la bienvenida! Puedes hacerlo de las siguientes maneras:

Creando nuevas funcionalidades.
Mejorando la documentación.
Reportando errores o problemas encontrados.
Para colaborar, simplemente crea un fork del repositorio, realiza tus cambios y envía un pull request.

Notas Adicionales
Asegúrate de tener instalado Java y Maven en tu sistema antes de ejecutar las aplicaciones.
Se puede integrar una base de datos lógica para almacenar datos relevantes para el sistema, como información de hoteles y ciudades.
¡Gracias por tu interés en este proyecto! Si tienes alguna pregunta o sugerencia, no dudes en contactarnos.