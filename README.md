# Document AI

Document AI es una plataforma de Google Cloud que permite extraer información de documentos de forma automática y escalable.

En este repositorio se encuentra el ejemplo de como sacar datos de una tabla de un documento PDF y guardarlos en un archivo CSV.

## Como utilizarlo

1. Clonar el repositorio
2. Instalar las dependencias con `pip install -r requirements.txt`
3. Crear un proyecto en Google Cloud y activar la API de Document AI
4. Crear un servicio de cuenta de servicio y descargar la clave en formato JSON
5. Renombrar el archivo JSON a `ServiceAccountToken.json` y colocarlo en la carpeta ./files
6. Modificar la ruta de la clave en el archivo `main.py` si es necesario
7. Modificar la ruta del archivo PDF en el archivo `main.py` si es necesario
8. Ejecutar el script con `python main.py` o ejecutandolo en el IDE


## TODO:

- [ ] Modificar la salida del script para que en vez de devolver un CSV por cada tabla, devuelva un único CSV con toda la tabla de datos de la factura. Tiene que ignorar las tablas que no sean de datos de la factura.