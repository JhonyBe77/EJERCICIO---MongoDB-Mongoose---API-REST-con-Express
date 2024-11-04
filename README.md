# 📦 API REST con Express, MongoDB y Mongoose

Este proyecto implementa una API REST con **Express** para gestionar **Proveedores** (`Providers`) y **Productos** (`Products`) en **MongoDB** utilizando **Mongoose**. La relación entre productos y proveedores está normalizada.

## 🚀 Requisitos Previos

- **Node.js** y **npm**
- **MongoDB** en funcionamiento
- **Postman** (opcional, para probar los endpoints)

## ⚙️ Instalación

1. Clona el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd <NOMBRE_DEL_REPOSITORIO>
   ```

2. Instala las dependencias:
   ```bash
   npm install
   ```

3. Configura la conexión a MongoDB en el archivo .env:
   ```bash
   MONGODB_URI=mongodb://localhost:27017/nombre_de_tu_base_de_datos
   PORT=5000
   ```
4. Inicia el servidor:
     ```bash
    npm start
   ```

## 📂 Estructura del Proyecto

- models/providers.js: Define el esquema y modelo de Provider con los campos company_name, CIF, address y url_web.
- models/products.js: Define el esquema y modelo de Product con relación al modelo Provider.
- routes/providers.js: Define las rutas CRUD para Provider.
- routes/products.js: Define las rutas CRUD para Product.
- server.js: Configura Express, los middlewares y las rutas de la API.
