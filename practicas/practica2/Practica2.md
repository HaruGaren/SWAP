# Pr�ctica 2: clonar la informaci�n de un sitio web

Lo primero que tuve que hacer (antes de empezar con la pr�ctica) fue cambiar los nombres de los usuarios de los servers (ten�a un nombre de usuario 
para cada servidor) al mismo, para seguir el consejo del profesor y evitarnos futuros quebraderos de cabeza. Para ello, desde root utilic� el comando
"usermod" para cambiarle el nombre tanto al usuario como a su directorio. Tambi�n tuve que cambiarle el nombre al grupo de los usuarios con "groupmod".

Una vez todos ten�an el mismo usuario, hice propietario al usuario de la carpeta "/var/www/" en ambos servidores.

Cre� en el ServidorWeb1 un archivo llamado "prueba" en la carpeta "/var/www/", para posteriores pruebas:

![](prueba.png "Fichero 'prueba' en ServidorWeb1")

Luego fui a instalar la herramienta rsync, pero creo recordar que ya estaba instalada. Comprob� con los comandos de rsync 
listados en el gui�n de la pr�ctica desde la m�quina 2, y efectivamente se copiaba dicho archivo.

Acto seguido, pas� a generar la clave en la m�quina 2 (tipo rsa), la copi� en la m�quina 1, le cambi� los permisos por si las moscas (eso en la m�quina1) 
y prob� a conectarme por ssh a ver si no me ped�a la clave. Los pasos se pueden ver en la siguiente imagen:

![](clave.png "Clave generada, copiada y login sin clave")

Prob� el comando final que iba a meter en el archivo "/etc/crontab/" para asegurarme de que funcionaba y que no me ped�a contrase�a:

![](rsync.png "rsync sin contrase�a")

Una vez cerciorado de que funciona, lo a�adimos al archivo para que se sincronice cada minuto. El archivo queda de la siguiente manera:

![](crontab.png "Archivo /etc/crontab/")

Y ya por �ltimo miramos que se sincronice correctamente, mirando que el archivo "prueba" se copie a la m�quina 2:

![](funcionando.png "Prueba de que funciona")

**P.D.:** la mayor�a del informe se hizo a posteriori, ya que hasta la clase de pr�cticas no sab�a que hab�a que ir documentando los pasos, 
creo que est� todo lo necesario, pero si hay algo que se me hubiera pasado fue por eso.