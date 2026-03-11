# Microservicio de Productos – Actividad 1 Fullstack III

## Descripción

Este proyecto corresponde al desarrollo de un **microservicio de gestión de productos** como parte de la **Actividad 1 de la asignatura Fullstack III**. El repositorio constituye dos partes:

Repositorio actual:
- Readme especifico
- Licencia
- Documento word con la parte escrita solicitada por la actividad
- Links a microservicios y repositorio de este mismo

Repositorio microservicio:
- Microservicio Producto con node
- Readme básico
- Licencia

El microservicio permite realizar operaciones básicas sobre productos mediante una **API REST**, incluyendo:

- Obtener todos los productos
- Obtener un producto por ID
- Crear un nuevo producto
- Eliminar un producto

La API fue desarrollada utilizando **Node.js** con **Express**, utilizando **PostgreSQL en NeonDB** como base de datos y desplegada en **Render**.  
La documentación de la API se encuentra disponible mediante **Swagger**.

---

# Tecnologías utilizadas

- Node.js
- Express
- PostgreSQL
- NeonDB
- Swagger (Documentación de API)
- Render (Deploy del microservicio)
- Postman (Pruebas de endpoints)

---

# Enlaces del proyecto

### Repositorio
https://github.com/NBello26/Microservicios-Actividad-1-FullStack-III.git

### API desplegada
https://microservicios-actividad-1-fullstack-iii-1quf.onrender.com

### Documentación Swagger
https://microservicios-actividad-1-fullstack-iii-1quf.onrender.com/api-docs/

---

# Endpoints disponibles

## Obtener todos los productos

**Método:** GET  

Endpoint:

```
/productos
```

URL completa:

```
https://microservicios-actividad-1-fullstack-iii-1quf.onrender.com/productos
```

---

## Obtener producto por ID

**Método:** GET  

Endpoint:

```
/productos/{id}
```

Ejemplo:

```
https://microservicios-actividad-1-fullstack-iii-1quf.onrender.com/productos/1
```

---

## Crear un producto

**Método:** POST  

Endpoint:

```
/productos
```

Body (JSON):

```json
{
  "nombre": "Mouse Gamer",
  "precio_clp": 25000,
  "descripcion": "Mouse RGB",
  "stock": 10
}
```

URL:

```
https://microservicios-actividad-1-fullstack-iii-1quf.onrender.com/productos
```

---

## Eliminar un producto

**Método:** DELETE  

Endpoint:

```
/productos/{id}
```

Ejemplo:

```
https://microservicios-actividad-1-fullstack-iii-1quf.onrender.com/productos/1
```

---

# Ejecución local

Para ejecutar el proyecto localmente:

## 1. Clonar el repositorio

```
git clone https://github.com/NBello26/Microservicios-Actividad-1-FullStack-III.git
```

## 2. Instalar dependencias

```
npm install
```

## 3. Configurar variables de entorno

Crear un archivo `.env` en la raíz del proyecto:

```
PORT=3000
DATABASE_URL=URL_DE_TU_BASE_DE_DATOS
```

## 4. Ejecutar el servidor

```
npm run dev
```

El servidor quedará disponible en:

```
http://localhost:3000
```

---

# Pruebas de la API

Los endpoints pueden probarse utilizando:

- Postman
- Swagger UI
- Curl
- Navegador web (para endpoints GET)

---

# Autor

**Nicolás Bello**  
**Rodrigo Vargas**
Actividad 1 – Fullstack III
