⚙️ Backend - API Estudiantes

Este proyecto es el backend de la aplicación Interfaz Estudiantil.
Está desarrollado en Spring Boot y expone una API REST para gestionar estudiantes (crear, listar, editar y eliminar).

🔽 Descargar colletion Postman : https://www.mediafire.com/file/womlucxacv1a2ld/Gts+Estudiantes.postman_collection.json/file


![WhatsApp Image 2025-09-30 at 4 45 41 PM](https://github.com/user-attachments/assets/5e1876e8-af3b-4e41-8b98-9af45171f306)
![WhatsApp Image 2025-09-30 at 4 46 04 PM](https://github.com/user-attachments/assets/99bd4eb7-9dd8-4711-9405-b981d5eefbf7)

El frontend (Angular) consume esta API para mostrar y manipular la información.

🚀 Tecnologías utilizadas

Java 17+

Spring Boot 3.x

Spring Data JPA (acceso a base de datos)

Spring Web (endpoints REST)

Base de datos: PostgreSQL / MySQL (según configuración)

Maven como gestor de dependencias

📂 Estructura del proyecto

![WhatsApp Image 2025-09-30 at 5 53 37 PM](https://github.com/user-attachments/assets/869a55a4-6951-4fa7-a73b-1b4ec357b66c)


⚙️ Instalación y ejecución

1️⃣ Clonar el repositorio
git clone 
cd backend-estudiantes

2️⃣ Configurar la base de datos

En application.properties o application.yml:

spring.datasource.url=jdbc:postgresql://localhost:5432/estudiantes
spring.datasource.username=postgres
spring.datasource.password=tu_clave

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect

3️⃣ Ejecutar el proyecto
./gradlew bootRun


Por defecto estará en:
👉 http://localhost:8090

🌐 Endpoints principales
Método	Endpoint	Descripción
POST	/api/student	Crear estudiante
GET	/api/student	Listar todos los estudiantes
GET	/api/student/{id}	Obtener estudiante por ID
PUT	/api/student	Actualizar estudiante
DELETE	/api/student/{id}	Eliminar estudiante
🛠️ Scripts útiles

./gradlew clean build → compila y empaqueta

./gradlew bootRun → ejecuta la app

./gradlew test → corre las pruebas unitarias

docker-compose up -d → levanta base de datos y servicios auxiliares
