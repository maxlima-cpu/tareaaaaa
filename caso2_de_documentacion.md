# Guía de usuario: Registro de un Nuevo Producto

## 1. Objetivo

### 1.1 Que permite realizar esta funcionalidad?

Esta funcionalidad permite al usuario registrar un producto nuevo en la base de datos del sistema de ventas e inventario de la empresa.

## 2. Información necesaria

Antes de iniciar el registro, asegúrese de contar con los siguientes datos del producto:

- Nombre comercial del producto.
- Código SKU o código de barras único.
- Categoría correspondiente (Electrónica, Abarrotes, Limpieza, etc.).
- Precio unitario de venta.
- Cantidad inicial en stock.

## 3. Procedimiento

### 3.1 : Ingresar al módulo de inventario

1. Inicie sesión en la plataforma con sus credenciales de usuario.
2. Diríjase al menú lateral izquierdo y haga clic en **"Inventario"**.
3. Seleccione el botón **"Nuevo Producto"**.

![Módulo de Inventario](https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=800&q=80)
### 3.2 : Llenar el formulario

1. Complete los campos obligatorios marcados con un asterisco (*).
2. Seleccione la categoría adecuada desde la lista desplegable.
3. Ingrese el precio numérico y el stock inicial.

### 3.3 : Guardar el registro

1. Verifique que la información ingresada sea correcta.
2. Haga clic en el botón **"Guardar Producto"**.

![Formulario de Registro](https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=800&q=80)
## 4. Resultado esperado

Al hacer clic en guardar, el sistema mostrará un mensaje de confirmación: `"Producto registrado exitosamente"`, y la lista de productos se actualizará automáticamente.

## 5. Errores frecuentes

- **Código SKU duplicado:** Ocurre si intenta registrar un producto con un código que ya existe en el sistema.
- **Campos obligatorios vacíos:** El sistema resaltará en color rojo los datos faltantes.

Estructura del mensaje de error retornado por la API:

```json
{
  "status": 400,
  "error": "Bad Request",
  "message": "El código SKU ingresado ya se encuentra registrado."
}