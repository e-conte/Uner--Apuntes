# Mecanismos de Protección en Sistemas Operativos

En este documento se explican los principales mecanismos de protección que implementan los sistemas operativos para evitar conflictos entre procesos y garantizar la seguridad del sistema.

---

## 1. Operación Dual (Modo Usuario y Modo Kernel)

Los sistemas operativos dividen la ejecución en dos modos:

- **Modo Usuario**:
  - Donde se ejecutan los procesos de usuario.
  - Acceso limitado a instrucciones y espacio de memoria asignado.
  
- **Modo Kernel (Supervisor)**:
  - Donde se ejecutan las rutinas del sistema operativo.
  - Permite ejecutar instrucciones privilegiadas para acceder al hardware.

**Control con Bit de Modo**:
- `Bit = 0`: Sistema en modo kernel.
- `Bit = 1`: Sistema en modo usuario.
  
**Proceso de Cambio**:
1. Un proceso realiza una llamada al sistema.
2. El bit cambia a modo kernel.
3. Se ejecuta la rutina correspondiente.
4. El sistema vuelve a modo usuario.

---

## 2. Protección de Dispositivos de Entrada/Salida

Los usuarios no tienen acceso directo a los dispositivos de E/S. En su lugar:

- **Solicitud al Sistema Operativo**:
  - Se realizan a través de **drivers**, que actúan como intermediarios entre el hardware y el sistema operativo.
  
- **Funciones de los Drivers**:
  - Definir operaciones que el hardware puede realizar.
  - Establecer la interfaz de comunicación con el sistema operativo.
  - Ejemplo: Drivers de impresoras (funciones comunes como "imprimir" o "notificar falta de papel", y funciones específicas como "imprimir a color").

---

## 3. Protección de Memoria

Para evitar que un proceso acceda a zonas de memoria no asignadas:

- **Registros Frontera**:
  - Indican el inicio y fin de la memoria asignada a un proceso.
  
- **Verificación de Acceso**:
  - El sistema operativo verifica que la dirección de memoria solicitada esté dentro de los límites.
  - Si el acceso es ilegal, se genera una interrupción y el sistema operativo toma medidas.

---

## 4. Protección del Procesador

Evita que un proceso monopolice el uso del procesador:

- **Quantum de Tiempo**:
  - En sistemas de tiempo compartido, cada proceso tiene un tiempo limitado (quantum) para ejecutarse.
  - Si un proceso no termina en ese tiempo, el sistema operativo lo desaloja y da paso a otro proceso.
  
- **Prioridades**:
  - Los sistemas operativos manejan prioridades para garantizar que los procesos más importantes se ejecuten primero, sin descuidar los de menor prioridad.

---

## Resumen

Los mecanismos de protección son esenciales para garantizar la seguridad y estabilidad del sistema operativo. Sin ellos, el sistema no podría funcionar de manera eficiente y segura.
