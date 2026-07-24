# El Buen Sabor - Rotiseria Web

Aplicacion web profesional para la rotiseria El Buen Sabor.

## Stack

- Frontend: HTML5, CSS3, JavaScript ES6+, Bootstrap 5, Font Awesome, Google Fonts
- Backend: Node.js, Express.js
- Base de datos: Firebase Firestore
- Imagenes: Firebase Storage

## Estructura

El proyecto se encuentra modularizado por capas:

- config: configuraciones globales (entorno y Firebase)
- controllers: controladores HTTP
- routes: definicion de rutas web y API
- middleware: control de errores y 404
- services: logica de negocio
- models: estructuras/modelos del dominio
- utils: utilidades reutilizables
- public: assets estaticos (css, js, img, icons)
- views: vistas HTML separadas por pantalla

## Requisitos

- Node.js 20+

## Instalacion

1. Instalar dependencias:

   npm install

2. Configurar variables en .env

3. Iniciar servidor:

   npm run dev

4. Abrir en navegador:

   http://localhost:3000

## Endpoints iniciales

- GET /api/health
- GET /api/contacto
- GET /api/categorias
- GET /api/categorias/:slug
- GET /api/categorias/:slug/productos

## Proximo roadmap

- Catalogo y productos desde Firestore
- Panel admin con CRUD y carga de imagenes en Firebase Storage
- Integracion de pedidos por WhatsApp

## Flujo implementado

- /categoria muestra todas las categorias en tarjetas (imagen + nombre)
- /categoria/:slug muestra productos de la categoria seleccionada
- Cada producto permite agregar una aclaracion opcional
- Las aclaraciones se guardan junto al item del carrito en localStorage
