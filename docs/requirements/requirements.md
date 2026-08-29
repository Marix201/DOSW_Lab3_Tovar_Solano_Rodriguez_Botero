# Requerimientos del Sistema

## 1. Lista general de requerimientos

El sistema de TechCup tiene los siguientes requerimientos (descripción a alto nivel):

### 1.1 Requerimientos funcionales

El sistema de TechCup debe tener la capacidad de:

- **RF-01:** Permitir a los organizadores crear un torneo especificando fechas, cuota de inscripción y demás información básica.
- **RF-02:** Permitir a los capitanes crear un equipo y registrarlo en el torneo activo.
- **RF-03:** Permitir a los capitanes realizar el pago de inscripción de su equipo a través de PSE.
- **RF-04:** Permitir a los organizadores validar y aprobar el pago de inscripción de un equipo.
- **RF-05:** Permitir a los organizadores generar un reporte de los equipos registrados en un torneo.

### 1.2 Requerimientos no funcionales

El sistema de TechCup debe tener:

- **RNF-01 (Seguridad):** Cifrado de las contraseñas de los usuarios almacenadas en la base de datos.
- **RNF-02 (Disponibilidad):** Disponibilidad de al menos el 99% del tiempo durante los períodos de inscripción de torneos.
- **RNF-03 (Usabilidad):** Una interfaz que permita a un capitán completar el registro de su equipo en menos de 5 minutos.
- **RNF-04 (Rendimiento):** Generación de los reportes de registro e ingresos en un tiempo no mayor a 5 segundos.
- **RNF-05 (Interoperabilidad):** Capacidad de enviar el reporte de pagos de inscripción a la Decanatura en formato JSON.

## 2. Diagramas de caso de uso

### 2.1 Requerimiento Funcional 1

| Campo | Descripción |
|---|---|
| ID | RF-01 |
| Nombre del requerimiento | Crear Torneo |
| Descripción | El sistema debe permitir a un organizador autenticado crear un nuevo torneo, especificando su fecha, la cuota de inscripción y demás información básica. |
| Precondiciones | Para que el sistema cumpla con este requerimiento, TechCup debe tener previamente al organizador autenticado y no debe existir un torneo con el mismo ID (año + semestre). |
| Actor | Organizador |
| Flujo principal | 1. El organizador inicia sesión en el sistema.<br>2. El organizador selecciona la opción "Crear torneo".<br>3. El sistema muestra un formulario solicitando fecha, cuota de inscripción y demás información básica.<br>4. El organizador diligencia los campos y confirma la creación.<br>5. El sistema valida que el torneo no exceda un día de duración y que el ID sea único.<br>6. El sistema crea el torneo con estado inicial "Pendiente" y lo almacena.<br>7. El sistema confirma la creación al organizador. |
| Diagrama de caso de uso | |
| Poscondiciones | Se espera como resultado un nuevo torneo creado con estado "Pendiente", disponible para su posterior activación. |

### 2.2 Requerimiento Funcional 2



### 2.3 Requerimiento Funcional 3



## 3. Preguntas


