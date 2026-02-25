# TuPrimeraPagina-MarioChiarvetti

Proyecto web en **Django** (patrón **MVT**) para la consigna “TuPrimeraPagina”.

## Consigna (cumplida)
✅ Herencia de plantillas (base.html)  
✅ 3 modelos en `models.py`  
✅ Formularios para cargar datos en los 3 modelos  
✅ Búsqueda en base de datos (con 1 modelo es suficiente)  
✅ CRUD (crear, editar, borrar, detalle)

---

## Requisitos
- Python 3.12+ (recomendado)
- Dependencias:

```bash
pip install -r requirements.txt
Cómo ejecutar el proyecto

Ir a la carpeta donde está manage.py (carpeta src/):

cd src

Crear y aplicar migraciones:

python manage.py makemigrations
python manage.py migrate

Levantar servidor:

python manage.py runserver

Abrir en el navegador:
http://127.0.0.1:8000/

Orden para probar funcionalidades (URLs)
1) Inicio

http://127.0.0.1:8000/

Desde el menú (navbar) se accede a Categorías, Productos y Proveedores.

2) Categorías (CRUD + búsqueda)

URL:

http://127.0.0.1:8000/producto/lista/

Acciones:

Crear categoría

Editar / Borrar / Ver detalle

Buscar por nombre usando el input Buscar...

3) Proveedores (CRUD)

URL:

http://127.0.0.1:8000/producto/proveedores/

Acciones:

Crear proveedor

Editar / Borrar / Ver detalle

4) Productos (CRUD)

URL:

http://127.0.0.1:8000/producto/productos/

Acciones:

Crear producto (requiere tener al menos 1 Categoría y 1 Proveedor cargados)

Editar / Borrar / Ver detalle

Listado muestra relación con Categoría y Proveedor

Archivos importantes

Herencia de plantillas:

core/templates/core/base.html

Navbar: core/templates/core/componentes/navbar.html

Modelos:

producto/models.py (Categoria, Proveedor, Producto)

Formularios:

producto/forms.py

Vistas y URLs:

producto/views.py

producto/urls.py
