📚 AppCursos – TP3

Aplicación .NET MAUI Blazor Hybrid con API REST para la gestión de cursos digitales.
Este trabajo práctico integra la app móvil del TP2 con una API propia en ASP.NET Core, permitiendo CRUD de usuarios, login con roles y sincronización entre frontend y backend.

✨ Características principales

API REST (ASP.NET Core)

Endpoints para Usuarios y Cursos.

CRUD completo expuesto vía Swagger.

Configuración de CORS para acceso desde la app móvil.

Login y Roles

Inicio de sesión validando credenciales contra la API.

Roles diferenciados: Admin y Usuario.

Restricciones de acceso en la UI según el rol.

Admin puede gestionar usuarios y cursos.

Gestión de Usuarios

Crear, editar, eliminar y listar usuarios.

Confirmación antes de eliminar.

Avatares con placeholder automático.

Gestión de Cursos

Listado de cursos desde la API.

CRUD accesible según permisos del usuario.

UI y Estilo

Diseño responsivo con Bootstrap 5.

Botones con íconos de bootstrap-icons.

Layout adaptado a dispositivos móviles.

Pantalla de login personalizada con logo.

🛠️ Tecnologías utilizadas
Frontend (Móvil)

.NET MAUI
 – interfaz multiplataforma

Blazor Hybrid
 – componentes web embebidos

Bootstrap 5
 – estilos y responsive design

C#
 – lógica principal

Backend (API)

ASP.NET Core 9
 – API REST

Entity Framework Core
 – acceso a datos

[SQL Server] – base de datos relacional

Swagger / Swashbuckle
 – documentación de endpoints

📂 Estructura del proyecto

AppCursos/ → Proyecto móvil (.NET MAUI Blazor Hybrid)
AppCursosAPI/ → API REST en ASP.NET Core
CursosDATA/ → Librería de modelos y acceso a datos compartidos

AppCursos/
│── Components/        → Componentes reutilizables
│── Pages/             → Vistas Razor (Login, Usuarios, Cursos)
│── Services/          → Servicios de negocio (Sesión, Usuarios, Cursos)
│── Shared/            → Layout y componentes compartidos
│── wwwroot/           → Recursos estáticos (css, imágenes, logo)

AppCursosAPI/
│── Controllers/       → Endpoints REST (Usuarios, Cursos)
│── Data/              → Contexto EF Core
│── Program.cs         → Configuración de la API

CursosDATA/
│── Models/            → Clases de dominio (Usuario, Curso, Rol)

🚀 Cómo ejecutar el proyecto

Clonar el repositorio:

git clone https://github.com/Leandr0-Moreira/AppCursos-TP3.git


Levantar la API:

Abrir AppCursosAPI en Visual Studio.

Ejecutar en perfil HTTP.

Swagger disponible en /swagger.

Ejecutar la App móvil (MAUI):

Abrir AppCursos.sln.

Seleccionar Windows Machine o emulador Android.

La app consumirá la API vía http://localhost:PUERTO.

👨‍💻 Autor

Leandro Moreira

📄 Licencia
Proyecto académico sin fines comerciales.
Distribuido bajo licencia MIT (LICENSE).