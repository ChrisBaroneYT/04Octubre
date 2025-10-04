📱 CRUD | Móviles
🧩 Descripción

CRUD | Móviles es una aplicación Android desarrollada en Kotlin que permite gestionar usuarios de manera sencilla y eficiente.
La app se conecta con Supabase como backend para almacenar la información y permite realizar todas las operaciones básicas de un sistema CRUD:

✏️ Crear nuevos usuarios
🔍 Buscar usuarios por identificación
✏️ Editar y actualizar información
❌ Eliminar usuarios
📤 Listar y consultar datos en tiempo real
🚀 Características principales

✅ Registro de nuevos usuarios
✅ Edición de datos con validación
✅ Eliminación segura con políticas RLS en Supabase
✅ Conexión a base de datos en la nube usando Supabase REST API
✅ Navegación sencilla e interfaz intuitiva en Android
✅ Botón directo para abrir Google desde la app

🛠️ Tecnologías utilizadas

Kotlin – Lenguaje principal de la app
Android Studio – Entorno de desarrollo
Supabase – Base de datos y backend en la nube
OkHttp – Cliente HTTP para consumir la API
JSON / REST API – Intercambio de datos
ViewBinding / XML Layouts – Interfaz de usuario
Navigation Component – Manejo de pantallas y rutas

📂 Estructura del Proyecto
📁 com.example.myapplicationarturocashfaster
│
├── MainActivity.kt               # Actividad principal
├── SupabaseManager.kt           # Conexión con Supabase y funciones CRUD
├── ui/                          # Layouts y vistas
│   ├── activity_main.xml
│   ├── content_main.xml
│   └── fragment_user.xml
├── res/layout/                  # Archivos de diseño en XML
│   └── ...
└── AndroidManifest.xml

⚙️ Configuración del Backend (Supabase)

Crear un proyecto en Supabase
Crear la tabla usuarios con el siguiente script SQL:
(Incluye campos como nombres_y_apellidos, identificacion, rol_usuario_*, etc.)
Activar Row Level Security (RLS) y agregar las políticas necesarias (select, insert, update, delete).
Obtener la URL del proyecto y la API Key desde Settings > API y colocarlas en SupabaseManager.kt:
private const val SUPABASE_URL = "https://tu-proyecto.supabase.co"
private const val SUPABASE_KEY = "tu_api_key"

📲 Uso de la App

Clona este repositorio:
git clone https://github.com/tuusuario/CRUD-Moviles.git
Abre el proyecto en Android Studio.
Configura tu URL y API Key de Supabase en SupabaseManager.kt.
Ejecuta la app en un emulador o dispositivo físico con Android 8.0+.

👤 Autor
Desarrollado por Chris – Proyecto de prácticas en desarrollo de aplicaciones móviles con Kotlin y Supabase 🚀
