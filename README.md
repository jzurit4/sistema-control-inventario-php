# Sistema Control de Inventario PHP

## 1. Descripción general

Sistema web desarrollado en PHP para la gestión de inventario. Permite administrar
categorías, productos, usuarios y movimientos de stock, facilitando el seguimiento
de entradas y salidas de productos dentro de una organización.

Este repositorio corresponde a la versión inicial del sistema entregado para fines
académicos y fue versionado con Git en un entorno Windows y publicado en GitHub
como parte del proceso de documentación y control de cambios del proyecto.

## 2. Funcionalidades principales

- Inicio de sesión de usuarios registrados mediante `login.php`.
- Página principal con navegación general del sistema.
- Gestión de categorías de productos.
- Gestión de productos del inventario.
- Gestión de usuarios del sistema.
- Control de stock mediante entradas y salidas de productos.
- Búsqueda y paginación para facilitar la revisión de registros.
- Uso de modales para registrar y editar información.
- Conexión a base de datos MySQL/MariaDB mediante archivos de configuración.

## 3. Tecnologías utilizadas

- PHP
- MySQL / MariaDB
- HTML5
- CSS3
- JavaScript
- AJAX
- Bootstrap [COMPLETAR SI APLICA]
- XAMPP para Windows
- Git for Windows
- GitHub

## 4. Requisitos de instalación en Windows

Antes de ejecutar el sistema, se requiere contar con:

- Windows 10 o Windows 11.
- XAMPP instalado, idealmente en `C:\xampp`.
- Apache y MySQL activos desde XAMPP Control Panel.
- Navegador web actualizado.
- Git for Windows, si se desea clonar o versionar el repositorio.
- Visual Studio Code u otro editor de código.

## 5. Instalación local en Windows

1. Clonar el repositorio desde GitHub:

```bash
git clone https://github.com/USUARIO/sistema-control-inventario-php.git
```

2. Copiar o dejar la carpeta del proyecto dentro de `htdocs` de XAMPP:

```text
C:\xampp\htdocs\sistema-control-inventario
```

3. Iniciar Apache y MySQL desde XAMPP Control Panel.

4. Abrir phpMyAdmin desde el navegador:

```text
http://localhost/phpmyadmin
```

5. Crear la base de datos correspondiente e importar el archivo SQL ubicado en:

```text
BD\simple_stock.sql
```

6. Revisar la configuración de conexión en:

```text
config\db.php
config\conexion.php
```

7. Abrir el sistema en el navegador:

```text
http://localhost/sistema-control-inventario/login.php
```

## 6. Configuración de base de datos

El sistema utiliza un archivo SQL llamado `simple_stock.sql`, ubicado en la carpeta
`BD`. Este archivo contiene la estructura necesaria para que el sistema funcione.

Parámetros a revisar en `config\db.php`:

```php
DB_HOST: [COMPLETAR]
DB_USER: [COMPLETAR]
DB_PASS: [COMPLETAR]
DB_NAME: [COMPLETAR]
```

> Nota: no subir credenciales reales o personales al repositorio. En un proyecto real,
> se recomienda usar variables de entorno o un archivo de configuración de ejemplo.

## 7. Estructura del proyecto

```text
sistema-control-inventario/
|-- ajax/          # Peticiones AJAX para categorias, productos, usuarios y stock
|-- BD/            # Script SQL de base de datos
|-- classes/       # Clases PHP, incluyendo Login
|-- config/        # Archivos de conexion a base de datos
|-- css/           # Hojas de estilo
|-- img/           # Imagenes y recursos graficos
|-- js/            # Archivos JavaScript
|-- libraries/     # Librerias auxiliares
|-- modal/         # Formularios modales del sistema
|-- login.php      # Pantalla de autenticacion
|-- producto.php   # Gestion de productos
|-- categorias.php # Gestion de categorias
|-- usuarios.php   # Gestion de usuarios
`-- stock.php      # Control de stock
```

## 8. Uso general del sistema

1. Ingresar al sistema desde `login.php`.
2. Acceder al menú principal.
3. Administrar categorías antes de registrar productos.
4. Registrar productos asociados a una categoría.
5. Gestionar usuarios del sistema.
6. Usar el módulo de stock para registrar entradas y salidas.
7. Utilizar las opciones de búsqueda y paginación para revisar información.

## 9. Control de versiones

Este proyecto utiliza Git como sistema de control de versiones. Algunos comandos
básicos usados durante la creación del repositorio fueron:

```bash
git init
git add .
git commit -m "chore: version inicial del sistema control de inventario en Windows"
git branch -M main
git remote add origin https://github.com/USUARIO/sistema-control-inventario-php.git
git push -u origin main
```

## 10. Autoría y contexto académico

- Estudiante: [COMPLETAR]
- Asignatura: [COMPLETAR]
- Docente: [COMPLETAR]
- Institución: [COMPLETAR]
- Fecha: [COMPLETAR]

## 11. Estado del proyecto

Versión inicial publicada en GitHub. El sistema queda disponible para futuras mejoras,
corrección de errores, documentación adicional y despliegue en ambientes controlados.

## 12. Licencia

Uso académico. Completar licencia si el proyecto será reutilizado o publicado fuera
del contexto de la asignatura.
