Bifurcación sobre proyecto gitstats
=========================================

Estos son algunos cambios personales que he agregado al proyecto [gitstats](http://gitstats.sourceforge.net/), que espero integrar próximamente.

###Cambios realizados:
	
 - Cambio de la hoja de estilo(`gitstats.css`).
 - Localización al español(código embedido en `gitstats`).

###Trabajo a futuro:

 - Localización en multi-idiomas(soporte archivos `.po`).
   - en\_UK
   - en\_US
   - es\_MX
 - Soporte multi-plantillas
 - Graficación de una linea de tiempo mediante la instrucción:   `git log --graph --oneline --all`

Como instalar:
----------------------------

Una vez descargado el proyecto la forma de instalar es mediante el archivo _MakeFile_ utilizando la instrucción `make` con el parametro _install_ como se muestra a continuación:

	sudo make install

Requiere de `gnuplot` y de otras dependencias, en caso de existir el paquete instalar desde repositorio para resolver dependencias:

	apt-get install gitstats

Ingresar a la carpeta del proyecto **gitstats**(descargado previamente) y copiar los siguientes archivos:

**Actualizamos el CSS**

	 sudo cp gitstats.css /usr/local/share/gitstats/gitstats.css
	 sudo chmod +r /usr/local/share/gitstats/gitstats.css
	 
**Actualizamos el script**

	 sudo cp gitstats /usr/bin/gitstats
	 sudo chmod +rx /usr/bin/gitstats
