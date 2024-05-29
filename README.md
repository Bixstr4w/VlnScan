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
Generar reportes con los resultados del análisis.

## Requisitos

- Python 3
- `nmap` instalado en el sistema
- Las siguientes bibliotecas de Python:
  - `Click`
  - `python-nmap`
  - `requests`
  - `scapy`
  - `paramiko`

## Instalación

### Windows

1. **Instalar Python y `pip`**
   
   Descarga e instala Python desde [python.org](https://www.python.org/downloads/). Asegúrate de marcar la opción "Add Python to PATH" durante la instalación.

2. **Instalar `nmap`**
   
   Descarga e instala `nmap` desde [nmap.org](https://nmap.org/download.html). Asegúrate de agregar `nmap` a tu PATH durante la instalación.

3. **Instalar las Dependencias**
   
   Abre un terminal (Command Prompt o PowerShell) y ejecuta:
   `pip install click python-nmap requests scapy paramiko`

### Linux y macOS

#### Instalar Python y pip

La mayoría de las distribuciones de Linux y macOS vienen con Python preinstalado. Muy importante que tengamos nmap instalado ya que la utilidad de python-nmap lo requiere. 

**En Linux:**

`sudo apt update
sudo apt install python3 python3-pip`

**En macOS:**
`python3 -m ensurepip --upgrade`

### Instalar nmap
**En Linux:**
`sudo apt install nmap`

**En macOS:**
`brew install nmap`

## Dependencias
`pip3 install -r requirements.txt`




   
