# Monorepositorio de E-Shop de Café - Repositorio Padre

Este es el repositorio principal que gestiona los componentes del backend y del frontend del MVP de la tienda de café.

## Nuevas Características Implementadas
1. **Diseño Premium y Mobile-First:**
   - Interfaz completamente responsiva con un menú de navegación tipo hamburguesa en dispositivos móviles.
   - Temática premium oscura basada en café (radial espresso gradients, glassmorphism y micro-interacciones hover).
2. **Tablero de Control de la Marca:**
   - Redirección predeterminada del rol `BRAND` a la página de Métricas (`/metrics`) al iniciar sesión.
3. **Flujo de E-Commerce Integrado:**
   - Nueva pestaña de **Tienda** (`/store`) con carrito de compras reactivo (soporta añadir, remover, y modificar cantidades).
   - Guardias de ruta (`ProtectedRoute`) restrictivos para el carrito, permitiendo acceso solo a `FARMER` y `CUSTOMER`.
4. **Tres Roles de Usuario:**
   - `FARMER`: Vende grano de café crudo y compra café procesado.
   - `BRAND`: Monitorea métricas y gestiona el inventario de productos terminados.
   - `CUSTOMER`: Compra productos procesados del catálogo de la tienda.

## Estructura del Proyecto

- `backend`: Servicio de API del backend (Express, GraphQL, MongoDB)
- `frontend`: Interfaz de usuario web (React, Vite, TypeScript)

## Requisitos Previos

- Node.js (versión 18 o superior)
- MongoDB ejecutándose localmente en el puerto 27017

## Instalación

Ejecuta el script de instalación en el directorio raíz para instalar las dependencias de todos los entornos:

```bash
npm run install:all
```

## Inicialización de la Base de Datos (Seed)

Puebla la base de datos con registros iniciales de prueba (usuarios con roles, transacciones, tendencias de precios y productos):

```bash
npm run seed:backend
```

## Ejecución de la Aplicación

Para ejecutar ambos entornos en modo desarrollo de forma simultánea:

1. Iniciar backend:
   ```bash
   npm run dev:backend
   ```
2. Iniciar frontend:
   ```bash
   npm run dev:frontend
   ```

## Compilación para Producción

Compila el código de producción para ambos entornos:

```bash
npm run build:all
```
