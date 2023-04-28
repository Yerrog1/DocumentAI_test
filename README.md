# Document AI

Document AI es una plataforma de Google Cloud que permite extraer información de documentos de forma automática y escalable.

En este repositorio se encuentra el ejemplo de como sacar datos de una tabla de un documento PDF y guardarlos en un archivo CSV.

## Como utilizarlo

Todos los

1. Clonar el repositorio
2. Instalar las dependencias con `pip install -r requirements.txt`
3. Crear un proyecto en Google Cloud y activar la API de Document AI
4. Cambiar la variable `project_id` en el archivo `main.py` por el ID del proyecto creado 
5. Crear un servicio de cuenta de servicio y descargar la clave en formato JSON
6. Renombrar el archivo JSON a `ServiceAccountToken.json` y colocarlo en la carpeta ./files
7. Modificar la ruta de la clave en el archivo `main.py` si es necesario en la variable `key_path`
8. Crear un procesador de formularios en Document AI y copiar el ID
9. Cambiar el atributo `processor_id` en el archivo `main.py` por el ID del procesador creado
10. Colocar el archivo que se quiere analizar en la carpeta ./files/pdf
11. Modificar la ruta del archivo PDF en el archivo `main.py` si es necesario en la variable `file_path`
12. Ejecutar el script con `python main.py` o ejecutandolo en el IDE
13. El resultado se guardará en la carpeta ./files/csv y por terminal se vera el resultado



## TODO:

- [ ] Modificar la salida del script para que en vez de devolver un CSV por cada tabla, devuelva un único CSV con toda la tabla de datos de la factura. Tiene que ignorar las tablas que no sean de datos de la factura.


