# Sistema de Gestión de Inventario (InventoryManager)

## 1. Descripción

`InventoryManager` es una aplicación diseñada para facilitar el control y registro de productos en tiempo real dentro de pequeñas y medianas empresas.

### 1.1 Objetivo

Automatizar la entrada, salida y consulta de stock para evitar discrepancias de inventario y optimizar la toma de decisiones comerciales.

## 2. Funcionalidades

- Registro y edición de nuevos productos con código de barras.
- Actualización de stock de manera automatizada.
- Búsqueda filtrada por categoría y nivel de stock.
- Generación de reportes periódicos en formato JSON.

## 3. Tecnologías utilizadas

- Node.js 
- Express.js
- SQLite3
- Markdown para la documentación técnica

## 4. Ejecución del proyecto

### 4.1 Pasos de ejecución

1. Clonar el repositorio localmente mediante Git.
2. Instalar las dependencias del proyecto ejecutando `npm install`.
3. Configurar las variables de entorno en el archivo `.env`.
4. Iniciar el servidor con el comando `npm start`.

## 5. Ejemplo de código

Servidor Express para gestionar la API de productos:

```javascript
const express = require('express');
const app = express();
const PORT = 3000;

app.get('/api/products', (req, res) => {
  res.json({ message: 'Obteniendo lista de productos...' });
});

app.listen(PORT, () => {
  console.log(`Servidor activo en http://localhost:${PORT}`);
});