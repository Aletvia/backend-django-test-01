# Point of sale test
Desarrollo de una API Rest que implementa un sistema de inventario de productos y órdenes.

## Instalación
Requerimientos:
- Entorno virtual (venv)
- Python 3.7, pip

### Entorno de Desarrollo

Este entorno permite realizar modificaciones en la API. 
Para ello es necesario crear un entorno virtual, donde se resguardan todas las paqueterías necesarias para el desarrollo 
en la plataforma:

1. Crear entorno virtual (_venv_)
```shell script 
virtualenv venv
```
2. Activar entorno virtual
```shell script
source venv/bin/activate
```
3. Instalar paqueterías
```shell script
(venv) pip install -r PATH/requirements.txt
```

Con estos pasos generamos el acceso a las bibliotecas necesarias para el desarrollo del proyecto.

1. Es necesario realizar las migraciones correspondientes ejecute el siguiente comando en la terminal dentro de la misma carpeta:
```shell script
python src/manage.py makemigrations
python src/manage.py migrate
```
2. Para ejecutar los test de la API, ejecute el siguiente comando en la terminal dentro de la misma carpeta:
```shell script
src/manage.py test src
```
3. Si todo se encuentra en orden, podrá observar la respuesta de la API en OK



**Endpoints disponibles:**

- Consultar productos
GET: http://127.0.0.1:8000/api/products/

- Consultar órdenes
GET: http://127.0.0.1:8000/api/orders/

- Insertar nuevo producto
POST: http://127.0.0.1:8000/api/products/create/

- Insertar nueva orden
POST: http://127.0.0.1:8000/api/orders/create/

- Consultar producto
GET: http://127.0.0.1:8000/api/products/retrieve/id/

- Consultar orden
GET: http://127.0.0.1:8000/api/orders/retrieve/id/

- Actualizar producto
PUT / PATCH: http://127.0.0.1:8000/api/products/update/id/

- Actualizar orden
PUT / PATCH: http://127.0.0.1:8000/api/orders/update/id/

- Eliminar producto
DELETE: http://127.0.0.1:8000/api/products/delete/id/

- Eliminar orden
DELETE: http://127.0.0.1:8000/api/orders/delete/id/

