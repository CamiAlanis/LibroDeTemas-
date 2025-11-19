# Proyecto: Sistema de Gestión de Libro de Temas
Este proyecto digitaliza el libro de temas, permitiendo registrar clases y gestionar los usuarios del sistema (docentes, preceptores y administradores).

## Tecnologías utilizadas

### *Frontend*
- *React* (con Vite)
- *JavaScript*
- *CSS*
- *HTML*

### *Backend*
- *Node.js*
- *Express*
- *JWT* (para autenticación)
- *Sequelize* (ORM)
- *MySQL* (base de datos)

## Estructura del proyecto
libro-de-temas/
│
├── backend/
│   ├── package.json
│   ├── node_modules
│   ├── src/
│   │   ├── app.js
│   │   ├── server.js
│   │   ├── config/
│   │   │   ├── db.js
│   │   ├── models/
│   │   ├── controllers/
│   │   ├── routes/
│   │   ├── middlewares/
│   │   └── utils/
│   ├── .env
│
└── frontend/
    ├── package.json
    ├── vite.config.js
    ├── node_modules
    ├── public/
    │   └── index.html
    └── src/
        ├── main.jsx
        ├── App.jsx
        ├── assets/
        ├── components/
        ├── pages/
        ├── routes/
        ├── services/
        ├── context/
        ├── hooks/
        └── styles/

# Instalación del proyecto
A continuación se detallan los pasos para instalar y ejecutar el backend y el frontend del sistema.

## 1. Backend (Node.js + Express + JWT + MySQL)

### Requisitos
- Node.js instalado
- MySQL instalado
- Base de datos creada (libro_temas)
  
### Instalación
1. Entrar a la carpeta del backend
cd backend

2. Inicializar el proyecto
npm init -y

3. Instalar las dependencias principales
npm install express sequelize mysql2 bcrypt jsonwebtoken cors dotenv multer

4. Instalar dependencias de desarrollo
npm install --save-dev nodemon

5. Crear el archivo .env con las siguientes variables
PORT=3001
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=tu_contraseña
DB_NAME=libro_temas
JWT_SECRET=tu_clave_secreta

6. Crear la base de datos vacía en MySQL
CREATE DATABASE libro_temas;

7. Ejecutar el servidor
npm run dev

## 2. Frontend (React + Vite)
1. Crear el proyecto con Vite
npm create vite@latest frontend

2. Entrar a la carpeta del proyecto
cd frontend

3. Instalar dependencias básicas
npm install

4. Instalar dependencias adicionales
npm install react-router-dom axios react-icons

7. Ejecutar el servidor
npm run dev
