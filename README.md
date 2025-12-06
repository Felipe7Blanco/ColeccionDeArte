# 🎨 ArtVoyage API – Plataforma de Colecciones de Arte

ArtVoyage es una API REST desarrollada en Java con Spring Boot para una plataforma web enfocada en la visualización, exploración y gestión de colecciones de arte mediante imágenes.
Los usuarios pueden crear colecciones, compartir imágenes por medio de URLs y explorar el contenido artístico de otros usuarios de forma pública.

El sistema cuenta con autenticación JWT, manejo de roles y rutas protegidas, y está preparado para ser consumido por un futuro frontend en React + Vite o Angular, con proyección a convertirse en un proyecto comercial o startup.

## 🚀 Características Principales

✅ Registro e inicio de sesión de usuarios
✅ Autenticación segura mediante JWT (Access Token)
✅ Protección de rutas por token
✅ Sistema de roles y permisos
✅ Roles disponibles: ADMIN, USER, ARTIST
✅ Creación de colecciones de arte
✅ Asociación de imágenes mediante URLs
✅ Visualización pública de colecciones de otros usuarios
✅ CRUD completo de entidades principales
✅ Arquitectura REST
✅ Preparado para integración con frontend

### 🛠️ Tecnologías Utilizadas

Java 17+

Spring Boot

Spring Security

JWT (JSON Web Token)

Spring Data JPA / Hibernate

PostgreSQL

Maven

Lombok

Postman

### 🔐 Seguridad y Autenticación

Autenticación basada en JWT (Access Token)

Solo están habilitadas sin token:

✅ Registro

✅ Login

Todas las demás rutas requieren token

Control de acceso basado en roles (ADMIN, USER, ARTIST)

Envío de token mediante header:

Authorization: Bearer TU_TOKEN
👤 Módulos del Sistema
Usuarios

Registro

Login

Asignación de roles

Autenticación segura

Colecciones

Crear colecciones

Editar colecciones

Listar colecciones propias

Visualizar colecciones de otros usuarios

Imágenes

Registro de imágenes mediante URL

Asociación a colecciones

Visualización desde el frontend

### 🔁 Flujo de Autenticación

El usuario se registra

Inicia sesión

El servidor retorna un Access Token JWT

El token se envía en cada petición protegida

El backend valida permisos según el rol

### ⚙️ Instalación y Configuración
1️⃣ Clonar el repositorio
git clone https://github.com/Felipe7Blanco/ColeccionDeArte.git
2️⃣ Configurar la base de datos (PostgreSQL)

Archivo:

application.properties

Ejemplo:

spring.datasource.url=jdbc:postgresql://localhost:5432/artvoyage
spring.datasource.username=postgres
spring.datasource.password=tu_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
3️⃣ Ejecutar el proyecto
mvn spring-boot:run
### 🧪 Pruebas con Postman

Registro de usuario

Inicio de sesión

Obtención del token JWT

Envío del token en cada request protegida

### 🧱 Arquitectura del Proyecto

Controllers

Services

Repositories

Entities

DTOs

Configuración de Seguridad (JWT)

Manejo de Roles

### 🌐 Futuro Frontend

Este backend está preparado para integrarse con:

⚛️ React + Vite

🅰️ Angular

Permitirá:

Visualización de colecciones

Perfiles públicos de artistas

Gestión de colecciones

Exploración de arte

### 🛣️ Features Planeadas (Próximas Versiones)

🚧 Sistema de likes
🚧 Sistema de comentarios
🚧 Sistema de seguidores
🚧 Perfiles de artista más completos
🚧 Monetización con anuncios
🚧 Despliegue permanente en la nube

### ☁️ Despliegue

El proyecto estuvo desplegado temporalmente en Render

Actualmente fuera de línea por limitaciones del plan gratuito

Se planea un despliegue permanente cuando se integre el frontend

### 📈 Estado del Proyecto

✅ Backend funcional y estable
🛠️ Frontend en planificación
🚀 En proyección como startup / proyecto comercial

### 👨‍💻 Autor

Andrés Blanco
Ingeniero de Sistemas – Recién egresado
📍 Colombia
🔗 GitHub: https://github.com/Felipe7Blanco
🔗 LinkedIn: https://www.linkedin.com/in/andr%C3%A9s-blanco-366021367/

⭐ Si este proyecto te parece interesante, ¡apóyalo con una estrella en GitHub!
