# Introducción a Git

## Descripción
Este proyecto es una práctica de introducción a Git y GitHub. Incluye un programa básico en Python (`HolaMundo.py`) que imprime un mensaje en pantalla. El objetivo de la práctica es familiarizarse con los conceptos básicos de Git, como la inicialización de un repositorio, la realización de commits, la configuración de un archivo `.gitignore`, y la conexión con un repositorio remoto en GitHub.

## Instrucciones de Uso
Para ejecutar el programa `HolaMundo.py`, sigue estos pasos:

1. Asegúrate de tener Python instalado. Puedes verificarlo con el comando:
   ```bash
   python --version
   ```

2. Ejecuta el programa con el siguiente comando:
   ```bash
   python HolaMundo.py
   ```
   
   Esto mostrará en pantalla el mensaje `Hola Git`.

## Comandos Utilizados
Aquí está el listado de comandos de Git utilizados a lo largo de la práctica:

```bash
# Inicializar el repositorio
git init

# Añadir archivos al área de preparación
git add HolaMundo.py

# Realizar un commit con mensaje
git commit -m "Mensaje del commit"

# Crear un archivo .gitignore para ignorar archivos específicos
touch .gitignore

# Añadir y verificar el repositorio remoto
git remote add origin https://github.com/Jedua/hola-mundo-python

#puede ser main dependiendo la version
git push -u origin master

# Verificar estado del repositorio
git status

```

## Notas sobre el archivo .gitignore
- **Propósito**: El archivo `.gitignore` se creó para evitar que ciertos archivos sean rastreados y subidos al repositorio. En este caso, se ignoraron todos los archivos con la extensión `.log` para evitar que archivos de depuración (como `debug.log`) se suban accidentalmente.
  
- **Archivos ignorados**: En `.gitignore`, añadimos la línea `*.log`, que indica a Git que ignore cualquier archivo con la extensión `.log` en el proyecto.

## Verificación
- **Salida esperada del programa**: Al ejecutar `HolaMundo.py`, el programa imprimirá en la consola el mensaje `Hola Git`.
  
- **Verificación de archivos ignorados**: Para confirmar que el archivo `debug.log` no se ha subido al repositorio, ejecuta el comando:
 
  En el repositorio remoto (en GitHub), no debería aparecer el archivo `debug.log`, lo cual confirme que `.gitignore` está configurado correctamente.
