# ApiBackend

Entorno de desarrollo:
- Visual Studio 2022 o superior
- .NET 8 o superior
- SQL Server

Especificaciones de la API:
La API debe manejar una entidad llamada Producto con los siguientes campos:
- Id (int, clave primaria, autoincremental)
- Nombre (string, obligatorio, máximo 100 caracteres)
- Precio (decimal, obligatorio, mayor a 0)
- Stock (int, obligatorio, mínimo 0)

# Instalación
Clonar el repositorio: 
git clone https://github.com/Antoain/ProyectoApi.git

Configurar la base de datos: 
- Asegúrate de que SQL Server esté corriendo.
- Modifica la cadena de conexión en appsettings.json:
"ConnectionStrings": {
  "TiendaApiConnection": "Data Source=ASUS;Initial Catalog=ProductosApi;Integrated Security=True;Encrypt=False;Trust Server Certificate=True"
}

Aplicar migraciones:
En la consola colocamos Add-Migration InitDb y luego update-Database

Ejecutar:
- GET /api/productos -> Obtener todos los productos
- GET /api/productos/{id} -> Obtener un producto por ID
- POST /api/productos ->  Agregar un nuevo producto
- PUT /api/productos/{id} -> Actualizar un producto
- DELETE /api/productos/{id} -> Eliminar un producto

Funcionamiento:
https://docs.google.com/document/d/1t8pvTH8NGMn7OF8UyXAaSvU9p5B-cTay_YCsBicuGe4/edit?usp=sharing

Autor: tb0822032023@unab.edu.sv
