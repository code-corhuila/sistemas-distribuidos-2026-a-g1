# Actividad 2: Diagrama de Arquitectura

## Proyecto: Gestión de Citas Inteligente

Se diseñó una arquitectura inicial basada en **microservicios**, donde cada componente del sistema tiene responsabilidades específicas y una base de datos independiente. Esta arquitectura permite escalabilidad, mantenimiento sencillo y tolerancia a fallos, características propias de los sistemas distribuidos.

---

# Arquitectura General del Sistema

El sistema está compuesto por:

- Un **Frontend** desarrollado en Angular
- Un **API Gateway** que centraliza las peticiones
- Varios **microservicios**
- Una **base de datos independiente por cada microservicio**

---

# Componentes del Sistema

## 1. Frontend

Tecnología:

- Angular

Responsabilidad:

- Interfaz de usuario
- Envío de solicitudes al sistema
- Visualización de datos
- Gestión de sesiones del usuario

---

## 2. API Gateway

Tecnología:

- Spring Cloud Gateway

Responsabilidad:

- Recibir todas las solicitudes del cliente
- Redirigir las solicitudes al microservicio correspondiente
- Centralizar la seguridad y el control de acceso
- Manejar el enrutamiento del sistema

Puerto típico:

8080

---

# Microservicios del Sistema

## 1. Users Service

Responsabilidad:

- Registro de usuarios
- Inicio de sesión
- Gestión de perfiles
- Autenticación de usuarios

Base de datos:

usersdb

Puerto típico:

8081

Datos almacenados:

- id_usuario
- nombre
- correo
- contraseña
- rol
- estado

---

## 2. Turnos Service

Responsabilidad:

- Solicitud de citas
- Consulta de citas
- Cancelación de citas
- Gestión de disponibilidad

Base de datos:

turnosdb

Puerto típico:

8082

Datos almacenados:

- id_turno
- fecha
- hora
- estado
- id_usuario

---

## 3. Notifications Service (Opcional para futuras versiones)

Responsabilidad:

- Enviar notificaciones al usuario
- Registrar eventos del sistema
- Informar cambios en citas

Base de datos:

notificationsdb

Puerto típico:

8083

Datos almacenados:

- id_notificacion
- mensaje
- tipo
- fecha
- estado

---

# Comunicación entre Componentes

El sistema utiliza comunicación basada en:

HTTP / REST

Flujo de comunicación:

Usuario → Frontend → API Gateway → Microservicio → Base de datos

Cada microservicio:

- Funciona de manera independiente
- Tiene su propia base de datos
- Puede escalar de forma individual

---

# Diagrama de Arquitectura (Representación)
## Diagrama de Arquitectura del Sistema

![Diagrama de Arquitectura](doc/diagrams/Diagrama de Arquitectura.jpeg)


---

# Número de Microservicios

El sistema inicialmente cuenta con:

3 microservicios

- Users Service
- Turnos Service
- Notifications Service (opcional)

---

# Base de Datos por Microservicio

Cada microservicio tiene su propia base de datos, siguiendo el principio:

Database per Service

Esto permite:

- Independencia
- Escalabilidad
- Seguridad
- Mantenimiento sencillo

---

# Ubicación del API Gateway

El API Gateway se ubica entre:

Frontend y Microservicios

Su función principal es:

Centralizar las peticiones y controlar el acceso al sistema.

---

# Justificación de la Arquitectura

Se eligió una arquitectura basada en microservicios porque:

- Permite dividir el sistema en componentes independientes
- Facilita el mantenimiento y la escalabilidad
- Reduce el impacto de fallos en el sistema
- Mejora la organización del desarrollo
- Es adecuada para sistemas distribuidos

---

# Tecnologías Utilizadas

Frontend:

Angular

Backend:

Java 17  
Spring Boot  
Spring Cloud Gateway  

Base de datos:

PostgreSQL

Contenedores:

Docker

Control de versiones:

Git  
GitHub

---

# Conclusión

La arquitectura definida permite construir un sistema distribuido escalable, modular y fácil de mantener. Cada microservicio cumple una función específica y cuenta con su propia base de datos, mientras que el API Gateway centraliza las solicitudes del cliente, garantizando una comunicación organizada entre los componentes del sistema.

