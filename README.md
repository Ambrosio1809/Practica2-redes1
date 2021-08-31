# Practica 2 GRUPO 9

   <p align="center">
    <img src="./Practica2/erick/encabezado.png" title="hover text">
   </p> 

---------------------------------------------------------------------------
### INTEGRANTES
- ERICK VALENZUELA
- FERNANDO AMBROSIO
- AARON JUAREZ 
- SOHANY LOPEZ
---------------------------------------------------------------------------
### HERRAMIENTAS UTILIZADAS
- Equipo.
    - 4 computadores con sistema operativo libre *"windows"*
    - 4 computadoras con sistema de virtualiacion *"virtual box"*
- Software.
    - Administradors VPNs *"OpenVPN"*
    - GNS3 instalados en los hosts físicos.
    - Software de virtualización (VMWare o Virtual Box) instalados y configurados para uso con GNS3.
- Plataforma
    - Google Cloud Plataform (GCP)
---------------------------------------------------------------------------
### DESCRIPCION DE LA PRACTICA
Configuracion y administracion de dispositivos de una infraestructura de red para una compañía, realizando el diseño de topología que será utilizado como infraestructura de red, configurandose para proveer comunicación de acuerdo a las necesidades que se indican.

La compañía cuenta con 3 departamentos: informática, contabilidad y ventas. Se debe proveer comunicación entre los usuarios del mismo departamento y con su servidor web, por ejemplo, los usuarios del departamento de ventas no se podrán comunicar con ningún otro departamento solamente con su departamento

   <p align="center">
    <img src="./Practica2/erick/vlan.png" title="hover text">
   </p>

- REQUISITOS
    - Garantizar que los equipos del departamento de ventas puedan comunicarse únicamente con el sitio web de ventas y otros equipos del propio departamento.
    - Garantizar que los equipos del departamento de contabilidad puedan comunicarse únicamente con el sitio web de contabilidad y otros equipos del propio departamento.
    - Garantizar que los equipos del departamento de informática puedan comunicarse únicamente con el sitio web de informática y otros equipos del propio departamento.
    - Entre el departamento de contabilidad, informática y ventas no debe haber comunicación.

- TOPOLOGIAS
 <p align="center">
    <img src="./Practica2/erick/topolo.png" title="hover text">
   </p>

---------------------------------------------------------------------------
### PASOS PARA CREACION DE UNA RED VLAN

La topología de la red sera simulada sobre máquinas físicas. Para ello se
implementaran dispositivos Cloud en *GNS3*.

 <p align="center">
    <img src="./Practica2/erick/gns3.png" title="hover text">
   </p>

1. Configuración de la máquina virtual de *GNS3* para poder utilizar VirtualBox o
VMWare
    * Para poder configurar *VIRTUAL BOX* de tal modo que se puede utilizar una maquina virtual en *GNS3* debemos descargar la VM de gns3 para el sistema operativo linux, esta maquina virutal de gns3 lo que permite es poder conectar gns3 con una maquina virtual que tenga el sistema cualquier sistema operativo y poder utlizarla en el software de simulacion y puede sar parte de nuestra topologia, para esto esta debera ser descargada en siguiente enlace:
        - [https://www.gns3.com/software/download-vm](https://www.gns3.com/software/download-vm)
    *En el enlace se mostrar la siguiente pantalla y debemos descargar la que dice VirtualBox en  su version mas actualizada
    
2. Configuración de las 2 topologías en GNS3
3. Configuración de las VPCs
4. Configuración de las máquinas virtuales
5. Instalación y configuración de los servidores web
6. Pings entre los clientes y entre los servidores web de los departamentos
correspondientes
7. Visualización de la página web desde el Host Virtual Cliente