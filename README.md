# es-keyboard-mapping-writers
Distribución de teclado para escritores de lengua española
----------------------------------------------------------

Esta distribución permite a los escritores de habla hispana obtener acceso fácil a los símbolos utilizados en la escritura de cuentos, novelas, etcétera.

Incluye la definición de los símbolos:
* «
* »
* "
* ¶
* §
* — (raya)

Para implementar esta definición de teclado:

Crear una copia de seguridad de la definición existente mediante el comando:

sudo mv /usr/share/X11/xkb/symbols/es /usr/share/X11/xkb/symbols/esbkp

Copiar el archivo "es" a la carpeta /usr/share/X11/xkb/symbols con el comando:

sudo cp es /usr/share/X11/xkb/symbols

Ejecutar la actualización de las definiciones mediante el comando:

sudo dpkg-reconfigure xkb-data

Es necesario ahora añadir una distribución distinta a «es» en la configuración (esto depende del entorno de escritorio); básicamente añadir una distribución alternativa del español, borrar la que estaba en uso y añadirla nuevamente, para que se reflejen los cambios.

