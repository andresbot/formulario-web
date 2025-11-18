# Sistema de Reclamos Web

Sistema web para gestión de reclamos, bugs y sugerencias. Permite a los usuarios reportar problemas y a los administradores gestionar los reportes.

## 📋 Descripción

Aplicación web que facilita la comunicación entre usuarios y trabajadores mediante un sistema de reportes. Los usuarios pueden enviar sus comentarios, y los trabajadores tienen acceso a un panel para revisar, gestionar y responder a los reportes.

## ✨ Características

### Para Usuarios
- **Registro e inicio de sesión** con validación de credenciales
- **Formulario de reclamos** con campos para tipo, nombre, correo y comentario
- **Interfaz responsive** adaptable a dispositivos móviles
- **Validación en tiempo real** de formularios

### Para Administradores
- **Panel de administración** con acceso controlado
- **Visualización completa** de todos los reclamos
- **Gestión de usuarios** registrados en el sistema
- **CRUD completo** para mensajes y usuarios

## 🛠️ Tecnologías Utilizadas

### Frontend
- HTML5, CSS3, JavaScript
- Font Awesome para iconos
- Diseño responsive sin frameworks

### Backend
- Node.js con Express
- MySQL para base de datos
- Arquitectura modular por servicios
- API RESTful

## 📁 Estructura del Proyecto

```
formulario-web/
├── frontend/
│   ├── index/          # Página principal y formulario
│   ├── login/          # Sistema de login
│   ├── registro/       # Registro de usuarios
│   ├── admin/          # Panel de administración
│   ├── usuario/        # Panel de usuario
│   └── assets/         # Estilos CSS
└── initial-backend/
    ├── src/
    │   ├── users/      # Módulo de usuarios
    │   └── messages/   # Módulo de mensajes
    ├── app.js          # Configuración de Express
    ├── config.js       # Variables de configuración
    └── db.js           # Conexión a base de datos
```

## 🚀 Instalación

1. Clonar el repositorio:
```bash
git clone https://github.com/andresbot/formulario-web.git
cd formulario-web
```

2. Instalar dependencias del backend:
```bash
cd initial-backend
npm install
```

3. Configurar la base de datos MySQL y actualizar las credenciales en `config.js`

4. Iniciar el servidor:
```bash
npm start
```

5. Abrir el frontend en un navegador o usar un servidor local

## 💻 Uso

1. **Registro**: Los nuevos usuarios pueden registrarse desde `/registro`
2. **Login**: Acceder con credenciales desde `/login`
3. **Enviar reclamo**: Completar el formulario en la página principal
4. **Administración**: Los administradores acceden a `/admin` para gestionar reportes

## 📝 API Endpoints

### Usuarios
- `GET /users` - Obtener todos los usuarios
- `GET /users/:id` - Obtener usuario por ID
- `POST /users/register` - Registrar nuevo usuario
- `POST /users/login` - Iniciar sesión
- `PUT /users/:id` - Actualizar usuario
- `DELETE /users/:id` - Eliminar usuario

### Mensajes
- `GET /messages` - Obtener todos los mensajes
- `GET /messages/:id` - Obtener mensaje por ID
- `POST /messages` - Crear nuevo mensaje
- `PUT /messages/:id` - Actualizar mensaje
- `DELETE /messages/:id` - Eliminar mensaje

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue o pull request para sugerencias o mejoras.

