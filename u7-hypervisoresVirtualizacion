# Guía Completa de Hipervisores y Virtualización

## Tabla de Contenidos
1. [Conceptos Básicos](#conceptos-básicos)
2. [Tipos de Hipervisores](#tipos-de-hipervisores)
3. [Máquinas Virtuales](#máquinas-virtuales)
4. [Modelo Cliente-Servidor](#modelo-cliente-servidor)
5. [Aplicaciones Prácticas](#aplicaciones-prácticas)
6. [Ventajas y Desventajas](#ventajas-y-desventajas)
7. [Glosario](#glosario)

---

## Conceptos Básicos <a name="conceptos-básicos"></a>

### ¿Qué es la Virtualización?
Tecnología que permite crear versiones virtuales de recursos físicos como servidores, almacenamiento y redes.

### ¿Qué es un Hipervisor?
Software que gestiona y distribuye recursos de hardware entre múltiples máquinas virtuales (VMs).

#### Funciones Clave:
- Aislamiento entre VMs
- Gestión de recursos (CPU, RAM, almacenamiento)
- Soporte para múltiples sistemas operativos

---

## Tipos de Hipervisores <a name="tipos-de-hipervisores"></a>

### Hipervisor Tipo 1 (Bare Metal)
| Característica | Ejemplos |
|---------------|----------|
| Ejecución directa sobre hardware | VMware ESXi, Hyper-V, Xen |
| Alto rendimiento | |
| Usado en entornos empresariales | |

### Hipervisor Tipo 2 (Hosted)
| Característica | Ejemplos |
|---------------|----------|
| Requiere SO anfitrión | VirtualBox, VMware Workstation |
| Fácil configuración | |
| Ideal para desarrollo/testing | |

---

## Máquinas Virtuales <a name="máquinas-virtuales"></a>

### Componentes de una VM
1. **vCPU**: Procesador virtual
2. **vRAM**: Memoria asignada
3. **Disco Virtual**: VMDK, VDI, etc.
4. **Interfaces de Red Virtual**

### Proceso de Creación
```mermaid
graph TD
    A[Seleccionar Hipervisor] --> B[Definir Especificaciones]
    B --> C[Crear Disco Virtual]
    C --> D[Instalar SO]
    D --> E[Configurar Red]
