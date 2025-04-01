# PPS-Unidad3Actividad2-PabloGil
Unidad 3 - Actividad 2. Detección de equipos, puertos, servicios,vulnerabilidades.

Tenemos como objetivo:

> Aprender y conocer comandos y herramientas para escanear y localizar equipos y recursos.
>
> Practicar y probar en el entorno de pruebas con dichas herramientas.
---
## ACTIVIDADES A REALIZAR
- Busca información de:
	- Como podemos obtener información pública con protocolo whois, web DoaminTools y DSNrecon.

	WHOIS: Es un protocolo que permite consultar la información registrada de un dominio o dirección IP, incluyendo datos del registrante, fechas de creación y expiración, entre 		otros. Puedes utilizar servicios en línea como 	el de ICANN para realizar estas consultas. ​

	DomainTools: Ofrece servicios avanzados de búsqueda WHOIS, proporcionando detalles sobre la propiedad de dominios, historial de direcciones IP, ranking, tráfico y más.

	DNSrecon: Es una herramienta utilizada para recopilar información DNS, como registros de zona, transferencias y otros datos relacionados con un dominio.​

   	# Uso de Herramientas de Seguridad para Búsqueda de Vulnerabilidades

	## 1. Cómo utilizar Nmap y Nikto para buscar equipos, puertos abiertos, servicios y vulnerabilidades

	### Nmap

	Nmap es una herramienta popular para realizar escaneos de redes y descubrir información sobre equipos, puertos abiertos y servicios.

	- Escanear una red completa para descubrir hosts activos:

	nmap -sn 192.168.1.0/24

	- Escanear puertos abiertos en un solo host:

	nmap 192.168.1.5

	- Escanear puertos específicos:

	nmap -p 22,80,443 192.168.1.5

	- Detectar servicios y versiones:

	nmap -sV 192.168.1.5

	### Nikto

	## Nikto: Nikto es una herramienta para escanear servidores web en busca de vulnerabilidades, configuraciones incorrectas y otros posibles problemas de seguridad. Un ejemplo 		básico de su uso sería:

	- Escanear un servidor web:

	nikto -h http://192.168.1.5

	## 2. Cómo utilizar Wfuzz, Dirb para localizar recursos web en servidores.

	### Wfuzz

	Wfuzz es una herramienta de fuzzing que se utiliza para descubrir recursos web ocultos (directorios, archivos, etc.). Aquí te dejo algunos ejemplos de cómo usarla:

  	**Fuzzing directorios y archivos en un servidor web:**
  	```bash
  	wfuzz -c -w /path/to/wordlist.txt -u http://192.168.1.5/FUZZ

	- Que scripts que podemos utilizar con Nmap para la búsqueda de vulnerabilidades.
	- Cómo podemos buscar información de explotación de vulnerabilidades con searchsploit
- Instala en tu navegador la extensión de Shodan y muestra la información que tenemos tanto de ip, como de dominio del sitio http://iesvalledeljerteplasencia.es 
- Sobre la red del laboratorio PPS con kali, bWAPP, Multidillae y DVWA:<
	- Ayudándote del fichero docker-compose localiza las diferentes máquinas y puertos que deberían de tener abiertos.
	- Identifica los equipos de la Red con Nmap.
	- Realiza análisis de puertos en las MV.
	- Encuentra los Servicios y Sistemas Operativos de las MV.
	- Inspecciona los puertos con nikto.
	- Busca las vulnerabilidades de las MV con los scripts de Nmap.
	- Localiza los servicios web que tienen las diferentes máquinas (Wfuzz y Dirb).
	- Utiliza el comando searchsploit para buscar información de explotación de vulnerabilidades presentes en linux con kernel 5
---	
## ENTREGA

>__Realiza las operaciones indicadas__

>__Crea un repositorio  con nombre PPS-Unidad3Actividad2-Tu-Nombre donde documentes la realización de ellos.__

> No te olvides de documentarlo convenientemente con explicaciones, capturas de pantalla, etc.

>__Sube a la plataforma, tanto el repositorio comprimido como la dirección https a tu repositorio de Github.__
