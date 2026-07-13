# Monorepositorio de E-Shop de Café - Repositorio Padre

Este es el repositorio principal que gestiona los componentes del backend y del frontend del MVP de la tienda de café mediante submódulos de Git.

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

Puebla la base de datos con registros iniciales de prueba (usuarios, transacciones, tendencias de precios y productos):

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
