# Actividad 1: Escribir User Stories

## Proyecto: Gestión de Citas Inteligente

Se definieron las siguientes **User Stories** utilizando el formato:

**Como [rol], quiero [acción], para [beneficio].**

Cada historia incluye sus **criterios de aceptación** y su **prioridad según la técnica MoSCoW**:

- **M (Must Have):** Debe tenerse obligatoriamente
- **S (Should Have):** Debería tenerse
- **C (Could Have):** Podría tenerse
- **W (Won’t Have):** No se tendrá por ahora

---

# User Stories del Sistema

---

## US-01 — Registro de Usuario

**Como** paciente,  
**quiero** registrarme en la plataforma,  
**para** poder acceder al sistema y solicitar citas.

### Criterios de aceptación:

- El sistema debe permitir ingresar nombre, correo y contraseña.
- El correo no debe repetirse.
- La contraseña debe almacenarse de forma segura.
- El usuario debe poder iniciar sesión después del registro.

**Prioridad:** Must Have

---

## US-02 — Inicio de Sesión

**Como** paciente,  
**quiero** iniciar sesión en el sistema,  
**para** acceder a mis funciones personales.

### Criterios de aceptación:

- El usuario debe ingresar correo y contraseña.
- El sistema debe validar las credenciales.
- Si son correctas, debe permitir el acceso.
- Si son incorrectas, debe mostrar un mensaje de error.

**Prioridad:** Must Have

---

## US-03 — Solicitar Cita

**Como** paciente,  
**quiero** solicitar una cita,  
**para** reservar un turno disponible.

### Criterios de aceptación:

- El sistema debe mostrar fechas y horarios disponibles.
- El usuario debe poder seleccionar un turno.
- El sistema debe guardar la cita.
- El turno no debe duplicarse.

**Prioridad:** Must Have

---

## US-04 — Ver Mis Citas

**Como** paciente,  
**quiero** ver mis citas programadas,  
**para** consultar mis turnos actuales.

### Criterios de aceptación:

- El sistema debe mostrar todas las citas del usuario.
- Debe mostrar fecha, hora y estado.
- Solo deben mostrarse las citas del usuario autenticado.

**Prioridad:** Must Have

---

## US-05 — Cancelar Cita

**Como** paciente,  
**quiero** cancelar una cita,  
**para** liberar un turno que ya no necesito.

### Criterios de aceptación:

- El usuario debe poder cancelar una cita.
- El estado debe cambiar a cancelada.
- El sistema debe confirmar la cancelación.

**Prioridad:** Must Have

---

## US-06 — Gestión de Usuarios

**Como** administrador,  
**quiero** gestionar usuarios del sistema,  
**para** controlar el acceso a la plataforma.

### Criterios de aceptación:

- El administrador debe poder ver usuarios registrados.
- Debe poder activar o desactivar usuarios.
- Debe poder consultar información de usuarios.

**Prioridad:** Should Have

---

## US-07 — Ver Todas las Citas

**Como** administrador,  
**quiero** ver todas las citas del sistema,  
**para** supervisar la operación general.

### Criterios de aceptación:

- El sistema debe mostrar todas las citas.
- Debe permitir filtrar por estado o fecha.
- Debe mostrar información clara y organizada.

**Prioridad:** Should Have

---

## US-08 — Notificaciones de Citas

**Como** paciente,  
**quiero** recibir notificaciones sobre mis citas,  
**para** estar informado de cambios en mis turnos.

### Criterios de aceptación:

- El sistema debe generar una notificación cuando se cree una cita.
- Debe generar notificación cuando se cancele una cita.
- La notificación debe mostrarse en el sistema.

**Prioridad:** Could Have

---

## US-09 — Actualizar Perfil

**Como** paciente,  
**quiero** actualizar mis datos personales,  
**para** mantener mi información actualizada.

### Criterios de aceptación:

- El usuario debe poder editar sus datos.
- El sistema debe validar la información.
- Los cambios deben guardarse correctamente.

**Prioridad:** Should Have

---

## US-10 — Reportes de Citas

**Como** administrador,  
**quiero** consultar reportes de citas,  
**para** analizar el uso del sistema.

### Criterios de aceptación:

- El sistema debe mostrar número de citas por día.
- Debe mostrar citas por estado.
- Debe permitir visualizar estadísticas básicas.

**Prioridad:** Could Have

---

# Priorización MoSCoW

## Must Have

- US-01 Registro de usuario
- US-02 Inicio de sesión
- US-03 Solicitar cita
- US-04 Ver citas
- US-05 Cancelar cita

## Should Have

- US-06 Gestión de usuarios
- US-07 Ver todas las citas
- US-09 Actualizar perfil

## Could Have

- US-08 Notificaciones
- US-10 Reportes

## Won't Have (por ahora)

- Pagos en línea
- Videollamadas médicas
- Inteligencia artificial para asignación automática
- Notificaciones por WhatsApp o SMS

---
