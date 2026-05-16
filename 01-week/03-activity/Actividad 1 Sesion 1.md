# 4. Actividades de Clase

## Actividad 1: Identificar Sistemas Distribuidos

### Instrucciones:
En grupos, identifiquen **3 aplicaciones** que usen a diario y clasifíquenlas:

- ¿Son monolíticas o distribuidas?
- ¿Qué pistas les dan para pensar eso?

Piensen en aspectos como:
- ¿Tiene aplicación móvil y versión web?
- ¿Funciona parcialmente sin conexión (offline)?
- ¿Sus funcionalidades parecen independientes entre sí?

### Ejemplo de Respuesta:

| Aplicación | Tipo de Sistema | Justificación |
|------------|----------------|---------------|
| WhatsApp | Distribuido | Tiene app móvil y web, maneja mensajería en tiempo real y servidores en la nube. |
| Netflix | Distribuido | Usa múltiples servicios como streaming, recomendaciones y gestión de usuarios. |
| Calculadora de Windows | Monolítico | Es una sola aplicación que funciona localmente sin depender de otros servicios. |



## Actividad 2: Formación de Equipos

### Instrucciones:
Formen equipos de **3 a 4 personas** y asignen roles iniciales.  
Los roles pueden rotar durante el semestre según las necesidades del proyecto.

### Roles Iniciales:

- **Tech Lead:**  
  Responsable de la arquitectura del sistema y decisiones técnicas.

- **Backend Developer:**  
  Encargado de la lógica del servidor, APIs y bases de datos.

- **Frontend Developer:**  
  Responsable de la interfaz de usuario y experiencia visual.

- **DevOps:**  
  Encargado del despliegue, integración continua y manejo de contenedores (Docker, CI/CD).

### Ejemplo de Registro de Equipo:

| Integrante | Rol Inicial |
|------------|-------------|
| Sofía Perafán | Tech Lead |
| Juan Pérez | Backend |
| María Gómez | Frontend |
| Carlos López | DevOps |

### Nota:
El equipo debe registrarse con el docente indicando:
- Nombre del equipo
- Integrantes
- Roles asignados



## Actividad 3: Brainstorming del Proyecto

### Instrucciones:
Cada equipo debe proponer **al menos 2 ideas de proyecto**.

Para cada idea deben responder:

- ¿Qué problema resuelve?
- ¿Qué microservicios necesitaría?
- ¿Qué datos maneja?

Luego, presentar las ideas al grupo para recibir retroalimentación.

---

### Idea de Proyecto 1: Sistema de Gestión de Citas Médicas Inteligente

**Problema que resuelve:**  
Dificultad para agendar citas médicas de manera rápida y organizada.

**Microservicios necesarios:**

- Servicio de Usuarios
- Servicio de Citas
- Servicio de Notificaciones
- API Gateway

**Datos que maneja:**

- Información de pacientes
- Horarios médicos
- Citas agendadas
- Estados de las citas



### Idea de Proyecto 2: Aplicación de Rutas Seguras

**Problema que resuelve:**  
Las aplicaciones actuales solo muestran la ruta más rápida, pero no consideran la seguridad de la zona.

**Microservicios necesarios:**

- Servicio de Geolocalización
- Servicio de Reportes de Incidentes
- Servicio de Usuarios
- Servicio de Análisis de Riesgo

**Datos que maneja:**

- Ubicación del usuario
- Historial de incidentes
- Zonas de riesgo
- Reportes de seguridad

---

## Conclusión

Estas actividades permiten comprender los conceptos básicos de los **sistemas distribuidos** y fomentar el trabajo en equipo para el desarrollo de proyectos basados en **microservicios**, facilitando la planificación inicial y la identificación de problemas reales que pueden resolverse mediante soluciones tecnológicas.
