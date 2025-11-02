## Instalación de NojeJS
Antes de comenzar es necesario instalar node.js
1. Ingresamos a la sigueinte liga:
```Node.js
https://nodejs.org/es
```
2. Damos click en el apartado de "Get Node.js"
<img width="707" height="182" alt="image" src="https://github.com/user-attachments/assets/595190a5-b68a-417e-a204-8cfc31dd4379" />

3. se nos abrira el apartado de descarga donde podremos seleccionar el tipo de descarga, el SO donde se va a descargar y usando chocolatey,
que es un complemento para ayudarnos a descargar ciertos paquetes

para instalar chocolatey sigue los siguientes pasos:

1. Si trataste de instalar chcocolatey y alguna carpeta pudo quedar corrupta usael siguiente comando en la terminal de power shell con privilegios de admin:
```Chocolatey
Remove-Item -Path "C:\ProgramData\chocolatey" -Recurse -Force
```
2. Una vez ejecutado, ingresamos el siguiente comando:
```
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```
Este comando va a permitir instalar y ejecutar scrips necesarios para la instalación solo en esa sesión

3. Lo siguiente es ingresar el comando:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
