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

	Nikto: Nikto es una herramienta para escanear servidores web en busca de vulnerabilidades, configuraciones incorrectas y otros posibles problemas de seguridad. Un ejemplo 		básico de su uso sería:

	- Escanear un servidor web:

	nikto -h http://192.168.1.5

	## 2. Cómo utilizar Wfuzz, Dirb para localizar recursos web en servidores.

	### Wfuzz

	Wfuzz es una herramienta de fuzzing que se utiliza para descubrir recursos web ocultos (directorios, archivos, etc.). Aquí te dejo algunos ejemplos de cómo usarla:

  	**Fuzzing directorios y archivos en un servidor web:**
  	```
  	wfuzz -c -w /path/to/wordlist.txt -u http://192.168.1.5/FUZZ
   	```

	## 3.Que scripts que podemos utilizar con Nmap para la búsqueda de vulnerabilidades.

	http-vuln-cve2014-3704: Busca la vulnerabilidad en Drupal conocida como CVE-2014-3704, que permite la ejecución remota de código.

	smb-vuln-ms17-010: Detecta la vulnerabilidad EternalBlue (CVE-2017-0144) en el protocolo SMB, que fue aprovechada por el ransomware WannaCry.

	ssl-heartbleed: Detecta la vulnerabilidad Heartbleed (CVE-2014-0160) en las implementaciones de OpenSSL.

	ftp-vsftpd-backdoor: Detecta si un servidor FTP vsftpd tiene una puerta trasera, conocida por la CVE-2011-2523.
   
	## 4.Cómo podemos buscar información de explotación de vulnerabilidades con searchsploit

	Para buscar un exploit relacionado con una vulnerabilidad específica, puedes usar el siguiente comando:

- searchsploit <término de búsqueda>

	Por ejemplo, si estás buscando un exploit para la vulnerabilidad Heartbleed, puedes usar:

- searchsploit heartbleed
	
	## 5. Instala en tu navegador la extensión de Shodan y muestra la información que tenemos tanto de ip, como de dominio del sitio http://iesvalledeljerteplasencia.
 
	![](images/1.JPG)

	![](images/2.JPG)

	![](images/3.JPG)

- Sobre la red del laboratorio PPS con kali, bWAPP, Multidillae y DVWA:<
	- Ayudándote del fichero docker-compose localiza las diferentes máquinas y puertos que deberían de tener abiertos.
   
   ![](images/3.3.png)
  
	- Identifica los equipos de la Red con Nmap.

   ![](images/3.4.png)
  
	- Realiza análisis de puertos en las MV.

   ![](images/3.5.png)

 	- Encuentra los Servicios y Sistemas Operativos de las MV.
 
   ![](images/3.6.png)

	- Inspecciona los puertos con nikto.

   ![](images/3.7.png)
  
	- Busca las vulnerabilidades de las MV con los scripts de Nmap.

   ![](images/3.8.png)
   
	- Localiza los servicios web que tienen las diferentes máquinas (Wfuzz y Dirb).

   ![](images/3.9.png)
  
	- Utiliza el comando searchsploit para buscar información de explotación de vulnerabilidades presentes en linux con kernel 5

   ![](images/4.png)
  
---	
## ENTREGA

>__Realiza las operaciones indicadas__

>__Crea un repositorio  con nombre PPS-Unidad3Actividad2-Tu-Nombre donde documentes la realización de ellos.__

> No te olvides de documentarlo convenientemente con explicaciones, capturas de pantalla, etc.

>__Sube a la plataforma, tanto el repositorio comprimido como la dirección https a tu repositorio de Github.__
