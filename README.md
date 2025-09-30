⚙️ Backend - API Estudiantes
![WhatsApp Image 2025-09-30 at 4 45 41 PM](https://github.com/user-attachments/assets/5e1876e8-af3b-4e41-8b98-9af45171f306)
![WhatsApp Image 2025-09-30 at 4 46 04 PM](https://github.com/user-attachments/assets/99bd4eb7-9dd8-4711-9405-b981d5eefbf7)

Este proyecto es el backend de la aplicación Interfaz Estudiantil.
Está desarrollado en Spring Boot y expone una API REST para gestionar estudiantes (crear, listar, editar y eliminar).

El frontend (Angular) consume esta API para mostrar y manipular la información.

🚀 Tecnologías utilizadas

Java 17+

Spring Boot 3.x

Spring Data JPA (acceso a base de datos)

Spring Web (endpoints REST)

Base de datos: PostgreSQL / MySQL (según configuración)

Maven como gestor de dependencias

📂 Estructura del proyecto
<img width="455" height="333" alt="image" src="https://github.com/user-attachments/assets/28a8bf1e-49f1-4da0-a306-44551ef0665d" />


⚙️ Instalación y ejecución
1️⃣ Clonar el repositorio
git clone https://github.com/tuusuario/backend-estudiantes.git
cd backend-estudiantes

2️⃣ Configurar la base de datos


spring.datasource.url=jdbc:postgresql://localhost:5432/estudiantes
spring.datasource.username=postgres
spring.datasource.password=tu_clave

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect

3️⃣ Ejecutar el proyecto



Por defecto se levanta en: http://localhost:8090

🌐 Endpoints disponibles
Método	Endpoint	Descripción
POST	/api/student	Crear estudiante
GET	/api/student	Listar todos los estudiantes
GET	/api/student/{id}	Obtener estudiante por ID
PUT	/api/student	Actualizar estudiante
DELETE	/api/student/{id}	Eliminar estudiante

Ejemplo de request JSON:

{
  "firstName": "Carlos",
  "lastName": "cordoba",
  "documentType": "CC",
  "document": "123456789",
  "age": 25,
  "email": "carlos@example.com",
  "state": "Activo",
  "createdAt": "2025-09-30T14:00:00",
  "updatedAt": "2025-09-30T14:00:00"
}

🛠️ Scripts útiles

mvn clean install → compila y empaqueta

mvn spring-boot:run → ejecuta la app

mvn test → corre las pruebas unitarias

👨‍💻 Autor

Backend desarrollado por Jhohan Palacios
Prueba técnica con Spring Boot + JPA + REST
