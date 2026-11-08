# TP Integrador – Virtualización con VirtualBox

**Materia:** Arquitectura y Sistemas Operativos
**Carrera:** Tecnicatura Universitaria en Programación (UTN)
**Integrantes:** JAVIER GUILLERMO PALACIOS – ABAUNZ LAUTARO

## Descripción
En este trabajo se instaló una máquina virtual con Ubuntu Server 24.04.5 LTS
usando Oracle VirtualBox 7.2.22 sobre Windows. En la máquina virtual se
configuró un servidor web Apache protegido con el firewall ufw, y se verificó
su funcionamiento accediendo desde otro dispositivo de la red local.

## Contenido del repositorio
- `informe/`: informe técnico del trabajo.
- `capturas/`: capturas de pantalla del proceso, numeradas en orden.
- `diagrama/`: diagrama de red (Packet Tracer).

## Entorno utilizado
- VirtualBox 7.2.22 sobre Windows
- Ubuntu Server 24.04.5 LTS (2 GB de RAM, 20 GB de disco)
- Red en modo adaptador puente

## Resumen del proceso
1. Instalación de VirtualBox y descarga de la imagen ISO de Ubuntu Server,
   verificando su integridad con SHA256.
2. Creación de la máquina virtual (2 GB de RAM, 20 GB de disco) con la red
   en modo adaptador puente.
3. Instalación de Ubuntu Server con OpenSSH. Se resolvió un error de
   virtualización activando AMD-V (SVM) en la BIOS.
4. Instalación de Apache y configuración del firewall (ufw), permitiendo
   OpenSSH y Apache.
5. Verificación del servicio: se accedió a http://192.168.0.63 desde un
   celular conectado a la misma red.
6. Creación de una instantánea (snapshot) de la VM ya configurada.
7. Diagrama de la red realizado en Cisco Packet Tracer.

## Referencias
- Universidad Tecnológica Nacional, Tecnicatura Universitaria en Programación a Distancia (2026).
  Unidad 7: Virtualización. Hipervisor tipo 1 y tipo 2. Arquitectura y Sistemas Operativos.
- Universidad Tecnológica Nacional, Tecnicatura Universitaria en Programación a Distancia (2026).
  Virtualización de recursos por un hipervisor Tipo 2. Arquitectura y Sistemas Operativos.
- Universidad Tecnológica Nacional, Tecnicatura Universitaria en Programación a Distancia (2026).
  Virtualización BIOS/UEFI. Arquitectura y Sistemas Operativos.
- Oracle. Oracle VM VirtualBox User Manual. https://www.virtualbox.org/manual/.
- Canonical. Ubuntu Server documentation. https://ubuntu.com/server/docs.
