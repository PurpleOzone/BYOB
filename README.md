# BYOB VM SIN PF

Configurar BYOB para usarse localmente con máquinas virtuales en Bridge:

Descargar el payload de Byob en formato Python y leerlo para analizarlo:

![image](https://user-images.githubusercontent.com/111320119/231361123-f68dcafa-10b9-45ea-9dd1-a8bf13547c0f.png)

En una terminal de Python, importa las librerias y copia el siguiente fragmento del archivo:
zlib.decompress(base64.b64decode(b'cadena en binario=='))

De esta manera, podremos decodificar la base 64 de lo que nos arroja dicho script.

![image](https://user-images.githubusercontent.com/111320119/231361950-daec6918-c5ac-4d2e-ae30-f1cbf6cfeeb2.png)


Dicho script nos arroja la dirección IP públic a la que se hace la petición, junto con el puerto al que hará la petición el bot una vez que se esté corriendo el script, copiamos el siguiente fragmento marcado en rojo incluyendo el puerto:

![image](https://user-images.githubusercontent.com/111320119/231361449-5b72b36e-1778-48ca-aaf0-36713b50c567.png)

Lo ingresamos en el navegador antecediento la IP donde se encuentra hosteada el BYOB. (tiene que estar en modo bridge la máquina virtual). Nos arrojará otro scipt de Python del que recuperaremos otra URL que modificaremos

Sintaxis:  http:// IP:1338 //stagers/nombrepayoad.py


![image](https://user-images.githubusercontent.com/111320119/231320343-923317d0-f87e-4e24-8218-8c2e21f4cf23.png)

Hasta el final de dicho archivo encontraremos la URL y recuperaremos lo siguiente:

![image](https://user-images.githubusercontent.com/111320119/231362671-6c7af6c2-ce53-4523-964d-7d33f2ff2dcf.png)

Realizamos la misma dinámica de extraer lo marcado en rojo y sustituir nuestra IP pública por la IP local de la máquina virtual. Encontraremos otro script de python que copiaremos en un bloq de notas por completo.


![image](https://user-images.githubusercontent.com/111320119/231321182-10db2e35-7198-4b71-8c93-cc9eb553e144.png)

Hasta el final basta con cambiar la ip pública a nuestra IP local en el espacio marcado en morado y guardar dicho archivo de Python. Este mismo quedará listo para ejecutarse en la víctima.

![image](https://user-images.githubusercontent.com/111320119/231321507-1bf44591-ff41-4d44-8e53-c61aa1dab828.png)

creditos: https://www.youtube.com/watch?v=9WqHuYP-vBA


## Manejo de errores
