# VlnScan

VlnScan es una utilidad de línea de comandos (CLI) desarrollada en Python para escanear vulnerabilidades en diferentes dispositivos de red. Utiliza `nmap` para escaneo de puertos, así como otras bibliotecas para realizar análisis detallados de servicios y configuraciones.

## Descripción

VlnScan permite escanear una variedad de dispositivos en busca de diferentes tipos de vulnerabilidades. La herramienta es extensible y modular, permitiendo agregar más tipos de escaneos y análisis según sea necesario.

## Alcance y Requisitos

### Tipos de Dispositivos a Analizar
- Routers
- PCs
- Servidores

### Tipos de Vulnerabilidades a Buscar
- Software desactualizado
- Puertos abiertos
- Configuraciones inseguras

### Métodos de Escaneo Utilizados
- Escaneo de puertos
- Análisis de servicios
- Revisión de configuraciones

## Selección de Bibliotecas y Herramientas

- `nmap`: Para escaneo de puertos y servicios.
- `requests` o `http.client`: Para realizar solicitudes HTTP y analizar respuestas.
- `scapy`: Para manipulación de paquetes de red.
- `paramiko`: Para conexiones SSH y revisión de configuraciones en dispositivos remotos.

## Diseño de la Arquitectura de la Aplicación

### CLI (Interfaz de Línea de Comandos)
Utilizo la biblioteca `Click` para crear una interfaz de línea de comandos amigable.

### Módulos de Escaneo
Módulos separados para diferentes tipos de escaneos (puertos, servicios, configuraciones).

### Reportes
Genera reportes con los resultados del análisis.

## Requisitos

- Python 3
- `nmap` instalado en el sistema
- Las siguientes bibliotecas de Python:
  - `Click`
  - `python-nmap`
  - `requests`
  - `scapy`
  - `paramiko`

## Dependencias
Para instalarlas todas juntas solo ejecutamos este comando:
`pip3 install -r requirements.txt`


## Asegurate de tener Python3, Pip3 y Nmap instalados.
### Ejecutar
`python3 vlnscan.py [options]`




   
