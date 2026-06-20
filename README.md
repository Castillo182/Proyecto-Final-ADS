# Proyecto-VER +
Ver+ - Plataforma de Monitoreo Visual Infantil

### Descripción
Ver+ es una plataforma web diseñada para apoyar el monitoreo visual infantil en niños de 0 a 3 años de edad.
El sistema permite a tutores, especialistas y administradores colaborar en la detección temprana de posibles alteraciones visuales mediante evaluaciones periódicas, seguimiento clínico, recomendaciones médicas y gestión de citas.

### Objetivo
Facilitar el seguimiento del desarrollo visual infantil mediante una plataforma centralizada que permita:

- Registrar perfiles infantiles.
- Realizar pruebas visuales rutinarias.
- Gestionar citas médicas.
- Llevar historial clínico.
- Generar recomendaciones personalizadas.
- Emitir reportes de seguimiento.
- Mantener comunicación entre tutores y especialistas.

### Tecnologías utilizadas

Frontend
- HTML5
- CSS3
- JavaScript ES6

Backend
- Supabase
  - PostgreSQL
  - Authentication
  - Row Level Security (RLS)
  - Functions (RPC)

### Librerías
- Lucide Icons
- Supabase JS


### Roles del sistema

Tutor

Puede:
- Registrar niños.
- Editar perfiles.
- Realizar pruebas visuales.
- Consultar historial.
- Solicitar asignación de doctor.
- Agendar citas.
- Ver recomendaciones.
- Descargar reportes.
- Acceder a la biblioteca digital.
  
Especialista
Puede:
- Consultar pacientes asignados.
- Revisar historial clínico.
- Registrar evaluaciones médicas.
- Generar recomendaciones.
- Configurar horarios disponibles.
- Gestionar citas.
- Agregar enlaces para videollamadas.

Administrador
Puede:
- Aprobar especialistas.
- Gestionar usuarios.
- Gestionar solicitudes de doctor.
- Asignar especialistas a pacientes.
- Supervisar el sistema.

### Funcionalidades implementadas

Tutores
- Dashboard de seguimiento.
- Gestión de perfiles infantiles.
- Pruebas visuales rutinarias.
- Historial de pruebas.
- Solicitud de especialista.
- Agenda de citas.
- Recomendaciones médicas.
- Biblioteca digital.
- Reportes PDF.

Especialistas
- Dashboard profesional.
- Gestión de pacientes.
- Evaluaciones médicas.
- Recomendaciones clínicas.
- Gestión de horarios.
- Videoconsultas.

Administrador
- Dashboard administrativo.
- Gestión de usuarios.
- Gestión de especialistas.
- Asignación de pacientes.
- Control de solicitudes.

### Estructura del proyecto

```text
Ver+
├── assets/
│   ├── img/
│   └── components/
│       ├── navbar.html
│       ├── footer.html
│       ├── paciente_sidebar.html
│       └── doctor_sidebar.html
│       └── admin_sidebar.html
├── css/
│   ├── base.css
│   ├── layout.css
│   ├── components.css
│   ├── dashboard.css
│   └── home.css
├── js/
│   ├── supabase.js
│   ├── cargarComponentes.js
│   ├── cargarPacienteSidebar.js
│   ├── cargarDoctorSidebar.js
│   └── cargarAdminSidebar.js
└── pages/
    ├── index.html
    ├── login.html
    └── registro.html
```

### Configuración del proyecto

1. Clonar repositorio
git clone URL_DEL_REPOSITORIO

2. Abrir proyecto
Puede utilizarse:
- Visual Studio Code
- Live Server
- XAMPP
- Cualquier servidor local

Ejemplo:
Open with Live Server

El proyecto se ejecutará normalmente en:
http://127.0.0.1:5500

Configuración de Supabase
Invitación al proyecto

Cada integrante debe:
1. Crear una cuenta en Supabase.
2. Proporcionar su correo institucional o personal.
3. Ser invitado por el propietario del proyecto.

Ruta:
Project Settings
→ Members
→ Invite Member

Permiso recomendado:
Developer

Conexión a la base de datos

Todos los integrantes deben utilizar el mismo archivo:
js/supabase.js

Ejemplo:
const supabaseUrl = "https://PROYECTO.supabase.co";
const supabaseKey = "PUBLIC_ANON_KEY";

export const supabase =
createClient(
    supabaseUrl,
    supabaseKey
);

No modificar estos datos sin autorización.

### Base de datos

El sistema utiliza PostgreSQL mediante Supabase.

Tablas principales:
- usuarios
- perfiles_ninos
- pruebas_visuales
- recomendaciones
- citas_especialistas
- solicitudes_doctor
- doctor_horarios
- evaluaciones_medicas
- biblioteca_educativa

Además se utilizan:
- Policies RLS
- Triggers
- Functions RPC

Flujo de citas
1. Tutor solicita especialista.
2. Administrador revisa solicitud.
3. Administrador asigna especialista.
4. Tutor visualiza horarios disponibles.
5. Tutor agenda cita.
6. Especialista confirma seguimiento.
7. Se puede realizar videollamada mediante enlace Meet.

Biblioteca digital
Incluye recursos educativos sobre:
- Desarrollo visual infantil.
- Señales de alerta.
- Estimulación visual.
- Seguimiento clínico.
- Recomendaciones para padres.

### Credenciales de prueba
Para facilitar las pruebas del sistema, se incluyen las siguientes cuentas de acceso:

Administrador

Correo: admin@gmail.com

Contraseña: 123456

Funciones disponibles:
- Gestión de usuarios.
- Gestión de especialistas.
- Aprobación de solicitudes.
- Asignación de especialistas a pacientes.
- Supervisión general del sistema.

Especialista

Correo: vic@gmail.com

Contraseña: 123456

Funciones disponibles:
- Consultar pacientes asignados.
- Registrar evaluaciones médicas.
- Generar recomendaciones.
- Gestionar horarios.
- Administrar citas.
- Configurar enlaces de videollamadas.

Tutor

Correo: nonbankstew@gmail.com

Contraseña: 123456

Funciones disponibles:
- Registrar perfiles infantiles.
- Realizar pruebas visuales.
- Consultar historial.
- Solicitar especialistas.
- Agendar citas.
- Consultar recomendaciones.
- Descargar reportes.
- Acceder a la biblioteca digital.

Nota: Estas cuentas fueron creadas únicamente para fines de demostración y evaluación académica del proyecto Ver+.

Las fuentes utilizadas corresponden a organizaciones médicas y científicas reconocidas.

### Integrantes
- ACOSTA MANCILLA CESAR ARMANDO
- LÓPEZ RAMOS MARCOS ISAID 
- MENDOZA CASTILLO ALEJANDRA

Licencia
Proyecto académico desarrollado para fines educativos.
© 2026 Ver+
