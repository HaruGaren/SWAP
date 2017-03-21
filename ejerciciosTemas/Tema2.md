*EJERCICIO T2.1: Calcular la disponibilidad del sistema si tenemos dos réplicas de cada elemento (en total 3 elementos en cada subsistema).* 

Aplicando las fórmulas del tema, los resultados son:

Elemento | Sin réplicas | 1 réplica | 2 réplicas
-------- | ------------ | --------- | ----------
Web | 0,85 | 0,9775 | 0,996625
Application | 0,9 | 0,99 | 0,999
Database | 0,999 | 0,999999 | 0,999999999
DNS | 0,98 | 0,9996 | 0,999992
Firewall | 0,85 | 0,9775 | 0,996625
Switch | 0,99 | 0,9999 | 0,999999
Data Center | 0,9999 | 0,9999 | 0,9999
ISP | 0,95 | 0,9975 | 0,999875
TOTAL | 0,598669721 | 0,9430193 | 0,992035952

Comprobados con un compañero que salió a hacer el ejercicio a la pizarra.



*EJERCICIO T2.2: Buscar frameworks y librerías para diferentes lenguajes que permitan hacer aplicaciones altamente disponibles con relativa facilidad.*

* PM2: como dice el enunciado, para desarrollar aplicaciones para Node.js
* Django: framework para Python.
* PHPOpenbiz: framework para PHP.



*EJERCICIO T2.3: 	¿Cómo analizar el nivel de carga de cada uno de los subsistemas en el servidor?* 

Con un programa especializado para ello (no se si era necesario contestar a esta pregunta).

*Buscar herramientas y aprender a usarlas.*

* ApacheBench: Esta herramienta como su nombre lo indica nos la entrega la fundación Apache y ofrece múltiples opciones, además viene preinstalada en los sistemas Mac OS X.
* Siege: Una herramienta utilizada ampliamente por desarrolladores (y algunos hacktivistas) para realización de pruebas de carga. Cortesía de JoeDog Software.

El cómo usarlas se puede mirar en la siguiente URL: http://codehero.co/como-hacer-pruebas-de-carga-servidores-web/

En cuanto a aprender a manejarlas, les he echado un vistazo, pero admito que no las he mirado exhaustivamente ni las he probado.




*EJERCICIO T2.4: Buscar ejemplos de balanceadores software y hardware (productos comerciales).*

* Nginx: balanceador software.
* Barracuda: balanceador hardware.

*Buscar productos comerciales para servidores de aplicaciones.*

* Microsoft .Net, Java EE, ...

*Buscar productos comerciales para servidores de almacenamiento.*
					
* Microsoft Azure, Amazon EC2, ...
