

# TALLER 3: TALLER MICROFRAMEWORKS-WEB-AREP


Programa creado para simular el microframework Spark a traves de funciones lambda.


### Prerequisitos

Para elaborar este proyecto se requirio de : 


Maven: Apache Maven es una herramienta que maneja el ciclo de vida del programa.



Git: Es un sistema de control de versiones distribuido (VCS).



Java 19: Java es un lenguaje de programación de propósito general orientado a objetos, portátil y muy versátil.



### Instalación

Clonamos el repositorio

```
    https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP

```
Se accede a la carpeta principal del repositorio repositorio que acabamos de clonar

	 cd MICROFRAMEWORKS-WEB-AREP

Hacemos la construccion del proyecto

	 mvn package
---
### Corriendo
Corremos los siguientes comando
	
	 mvn clean package install
	 mvn clean install

Ahora corremos el servidor
	
**Windows**

	 mvn exec:java -"Dexec.mainClass"="edu.escuelaing.arep.ASE.app.HTTPserver.webServer"

**Linux/MacOs**

	 mvn exec:java -Dexec.mainClass="edu.escuelaing.arep.ASE.app.HTTPserver.webServer"

Por ultimo accedemos a nuestro navegador con la siguiente URL

	 http://localhost:35000/

Aqui nos debera de cargar la siguiente pagina, con la cual podemos empezar a hacer las diferentes busquedas. 

![image](https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP/assets/98216991/95980164-ab29-4011-b882-6fbbca3994fb)


# Documentos HTML

![image](https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP/assets/98216991/e75d3489-78c8-4928-a82f-a238a4f2f3b8)


# Documentos CSS

![image](https://github.com/franciscoMarquezBocanegra/TALLER-DISE-O-Y-ESTRUCTURACI-N-DE-APLICACIONES-DISTRIBUIDAS-EN-INTERNET/assets/98216991/7e7fb204-3b3a-479a-bcd4-218fc17cc9d4)


# Documentos JS

![image](https://github.com/franciscoMarquezBocanegra/TALLER-DISE-O-Y-ESTRUCTURACI-N-DE-APLICACIONES-DISTRIBUIDAS-EN-INTERNET/assets/98216991/048115b9-617b-47d9-8883-59d8d307e653)



# Documentos JPG


![image](https://github.com/franciscoMarquezBocanegra/TALLER-DISE-O-Y-ESTRUCTURACI-N-DE-APLICACIONES-DISTRIBUIDAS-EN-INTERNET/assets/98216991/9030c4be-5970-4c8a-9935-c2a95d986b5d)



# Documentos aplicacion HTML CSS Y JS


![image](https://github.com/franciscoMarquezBocanegra/TALLER-DISE-O-Y-ESTRUCTURACI-N-DE-APLICACIONES-DISTRIBUIDAS-EN-INTERNET/assets/98216991/720884e5-f7f8-41aa-84a2-abfedcd662ac)



# Aplicacion de servicio REST


![image](https://github.com/franciscoMarquezBocanegra/TALLER-DISE-O-Y-ESTRUCTURACI-N-DE-APLICACIONES-DISTRIBUIDAS-EN-INTERNET/assets/98216991/319c39bf-b8dc-4149-a4e6-d2c80841f3ee)


# SO Windows 

![image](https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP/assets/98216991/750e1e45-587c-4084-852c-622a641f25cc)


# SO Linux

![image](https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP/assets/98216991/8158c83a-a9ec-47b4-bbaf-980d627b7ca8)



# ¿Como el desarrollador crearia una aplicacion con este marco de trabajo?

Es simple, debe primero crear un controlador para poder añadir los endpoints a la estructura de datos encargada de buscar el metodo correspondiente y implementar las funciones lambda para manejar el request, en este caso creamos este controlador. 


![image](https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP/assets/98216991/4cc9680c-3df3-4773-92f6-3000c42a0542)



 y luego debemos instanciar el controlador dentro del servidor web.


![image](https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP/assets/98216991/dfaf21aa-a3c4-4741-ad0c-0cf1ca383289)



con esto al poner a correr el servidor, y buscar el endpoint a traves de nuestro navegador nos saldra asi.


![image](https://github.com/franciscoMarquezBocanegra/MICROFRAMEWORKS-WEB-AREP/assets/98216991/b686bed5-233a-4259-be0e-f755d69e0f91)




---
### Corriendo test

Ejecutamos el comando

	mvn test
	
---


### Arquitectura del programa.


El programa está compuesto por diversas capas, cada una con su propia función específica:

## HTTPserver


La capa HTTPserver actúa como punto de entrada para las solicitudes entrantes, dirigiéndolas hacia las partes apropiadas del programa.

## Controllers


La capa de Controllers se encarga de recibir las solicitudes del servidor y de dirigirlas hacia los servicios correspondientes, actuando como intermediarios entre el servidor y la lógica de negocio.

## Services


La capa de Services contiene la lógica de negocio y se ocupa de realizar las operaciones requeridas por las solicitudes del usuario.

## ExternalWebServices


La capa ExternalWebServices se dedica a interactuar con servicios web externos, permitiendo a la aplicación acceder a recursos y funcionalidades fuera de su alcance directo.

## Static


La capa Static almacena archivos estáticos como HTML, JS, CSS y archivos de imagen. Estos archivos se sirven a los usuarios para presentar la interfaz de usuario en sus navegadores.



Esta estructura de capas facilita la organización, mantenimiento y escalabilidad del programa al separar las responsabilidades en componentes claros y definidos.



## Autor
*  Francisco Marquez
