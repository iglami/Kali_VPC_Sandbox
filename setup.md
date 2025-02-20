# Preparación del Entorno

## Hardware

- **CPU**: Xeon E5 2699 V3
- **Memoria**: 64GB DDR4, 3200MHz
- **Placa Base**: LGA 2011
- **Almacenamiento**: Asegúrate de tener suficiente espacio para las VM y los registros de pruebas.

## Instalación del Hypervisor

1. **Proxmox VE**:
   - Descarga Proxmox VE desde [Proxmox VE Downloads](https://www.proxmox.com/en/downloads).
   - Sigue las instrucciones de instalación en [Proxmox VE Documentation](https://pve.proxmox.com/wiki/Main_Page).

2. **VMware ESXi**:
   - Descarga VMware ESXi desde [VMware ESXi Downloads](https://customerconnect.vmware.com/en/group/vmware/evalcenter?p=free-esxi7).
   - Sigue las instrucciones de instalación en [VMware Documentation](https://docs.vmware.com/en/VMware-vSphere/index.html).

## Configuración de la Red Virtual

1. **Red Interna (LAN)**:
   - Configura una red interna para la comunicación entre las máquinas virtuales.
   
2. **Red Externa (WAN)** (opcional):
   - Configura una red externa si necesitas acceso a internet.

## Creación de Máquinas Virtuales

1. **Servidor de Firewall**:
   - **OS**: OPNsense o pfSense.
   - **Asignación de Recursos**: 4 vCPU, 8GB RAM, 20GB almacenamiento.

2. **Máquinas Objetivo (White Box)**:
   - **OS**: Windows, Linux (distintas distribuciones).
   - **Asignación de Recursos**: Dependiendo de las necesidades específicas de cada máquina.

3. **Máquina de Ataque (Kali Linux)**:
   - **OS**: Kali Linux.
   - **Asignación de Recursos**: 4 vCPU, 8GB RAM, 20GB almacenamiento.
