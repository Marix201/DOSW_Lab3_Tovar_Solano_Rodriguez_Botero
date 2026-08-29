# Requerimientos del Sistema

## 1. Sistema

**Nombre del sistema:** TechCup

**Objetivo:** El sistema tiene como objetivo permitir la gestión del torneo de fútbol organizado cada semestre entre los programas de Ingeniería de Sistemas, Ingeniería en Inteligencia Artificial, Ingeniería en Ciberseguridad e Ingeniería Estadística de la Escuela Colombiana de Ingeniería Julio Garavito, facilitando la creación de torneos, el registro de equipos, el procesamiento y validación de los pagos de inscripción, y la generación de reportes para organizadores y la Decanatura.

## 2. Problema a resolver

Actualmente la Escuela no cuenta con un sistema centralizado que permita crear torneos definiendo sus reglas básicas, registrar equipos de forma sencilla, procesar y validar los pagos de inscripción, consultar los equipos registrados por torneo, generar reportes de inscripción e ingresos, y enviar el reporte de pagos a la Decanatura en formato JSON. Esto obliga a manejar el proceso de forma manual y dispersa, generando riesgo de errores e inconsistencias entre estudiantes, capitanes y organizadores.

## 3. Diagrama de Contexto

### 3.1 Diagrama



Enlace al diagrama editable: https://lucid.app/lucidchart/cb0ab0fc-ff92-4376-b86a-30b40a68f413/edit?view_items=XnipXXKCii.I&page=0_0&invitationId=inv_d14314eb-c4ae-4291-a349-32dccf4a0078

### 3.2 Actores

| Actor / Rol | Descripción |
|---|---|
| Estudiante | Usuario autenticado del sistema. El caso de estudio no le da funcionalidades propias más allá de autenticarse; se asume acceso de solo consulta mientras no sea capitán de un equipo. |
| Capitán de equipo | Estudiante que además crea su equipo, actualiza su información, lo registra en el torneo activo y realiza el pago de inscripción. |
| Organizador | Usuario que crea y administra torneos, valida pagos y genera los reportes. |

### 3.3 Sistemas externos

| Sistema | Descripción |
|---|---|
| PSE | Pasarela externa de pagos utilizada para procesar el pago de la inscripción de un equipo. |
| Decanatura | Área de la Escuela que recibe el reporte de pagos de inscripción en formato JSON. |

## 4. Alcance del sistema

### 4.1 Dentro del sistema

- Autenticación de usuarios (organizadores y estudiantes/capitanes) mediante usuario y contraseña.
- Creación y gestión de torneos: fechas, cuota de inscripción, estado y demás información básica.
- Creación, actualización de información y registro de un equipo en el torneo activo.
- Pago de la inscripción de un equipo a través de PSE.
- Consulta, validación y aprobación del pago de inscripción por parte de un organizador.
- Generación de reportes de equipos registrados y de ingresos por inscripción.
- Envío del reporte de pagos de inscripción a la Decanatura en formato JSON.
- Eliminación de un torneo únicamente cuando no tiene equipos con pago aprobado (ver análisis de contradicciones en la Parte 3).

### 4.2 Fuera del sistema

- Gestión de partidos, calendario deportivo o resultados del torneo.
- Implementación de una pasarela de pagos propia (se delega completamente en PSE).
- Aplicación móvil nativa (solo se contempla la interfaz web).
- Notificaciones automáticas por correo o push.
