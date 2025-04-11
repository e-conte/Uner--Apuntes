# Comandos útiles en la terminal

## Comandos generales

### `echo`
Muestra un mensaje por pantalla.  
**Uso**:  
```bash
echo "mensaje"
Puede usarse con comillas dobles, simples o sin comillas, excepto cuando se utilizan variables de entorno.

Ejemplo con variable de entorno:

bash
Copy
echo $USER  # Muestra el nombre del usuario actual.
clear
Limpia la pantalla de la terminal.
Uso:

bash
Copy
clear
alias
Crea un atajo para un comando largo o complejo.
Uso:

bash
Copy
alias nombre_alias="comando"
Ejemplo:

bash
Copy
alias ls3="ls -l ~/facultad/tercero"
Para listar todos los alias definidos:

bash
Copy
alias
Reinicio y apagado de la PC
shutdown
Permite apagar, reiniciar o programar estos eventos.

Opciones principales:
Reiniciar inmediatamente:

bash
Copy
sudo shutdown -r now
Apagar inmediatamente:

bash
Copy
sudo shutdown now
Programar apagado en X minutos:

bash
Copy
sudo shutdown +10  # Apaga en 10 minutos.
Programar apagado a una hora específica:

bash
Copy
sudo shutdown 18:00  # Apaga a las 18:00.
Cancelar un apagado programado:

bash
Copy
sudo shutdown -c
Administración básica de procesos
ps
Lista los procesos en ejecución, mostrando información como el PID (Process ID).
Uso:

bash
Copy
ps
Para ver todos los procesos del sistema:

bash
Copy
ps -aux
kill
Finaliza un proceso enviándole una señal.
Uso:

bash
Copy
kill PID  # Reemplazar "PID" con el ID del proceso.
Para forzar la terminación de un proceso que no responde:

bash
Copy
kill -9 PID
Uso del editor de texto nano
Crear o editar un archivo
bash
Copy
nano nombre_archivo
Si el archivo no existe, se crea; si existe, se abre para edición.

Comandos básicos en nano:
Guardar: Ctrl + O (confirmar con Enter).

Salir: Ctrl + X.

Buscar texto: Ctrl + W.

Ejemplo práctico:
Editar un archivo existente:

bash
Copy
nano programa2020
Realizar cambios y guardar con Ctrl + O.

Salir con Ctrl + X.

Resumen final
Estos comandos son esenciales para trabajar eficientemente en la terminal, desde la administración de procesos hasta la edición de archivos y el control del sistema. Practicar su uso facilitará la realización de tareas avanzadas en entornos basados en línea de comandos.

