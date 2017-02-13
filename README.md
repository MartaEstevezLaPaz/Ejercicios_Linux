# Ejercicios_Linux

1.-Listar todos los archivos del directorio bin.
ls /bin

2.-Listar todos los archivos del directorio tmp.
ls /tmp

3.-Listar todos los archivos del directorio etc que empiecen por t en orden inverso.
ls -r /etc/t*

4.-Listar todos los archivos del directorio dev que empiecen por tty y tengan 5 caracteres.
ls /dev/tty??

5.-Listar todos los archivos del directorio dev que empiecen por tty y acaben en 1,2,3 ó 4.
ls /dev/tty*[1-4]

6.-Listar todos los archivos del directorio dev que empiecen por t y acaben en C1.
ls /dev/t*C1

7.-Listar todos los archivos, incluidos los ocultos, del directorio raíz.
ls -a /

8.-Listar todos los archivos del directorio etc que no empiecen por t.
ls /etc/[^t]*

9.-Listar todos los archivos del directorio usr y sus subdirectorios.
ls -l /usr

10.-Cambiarse al directorio tmp, crear directorio PRUEBA.
cd /tmp
mkdir PRUEBA

11.-Verificar que el directorio actual ha cambiado.
pwd

12.-Mostrar el día y la hora actual.
date

13.-Con un solo comando posicionarse en el directorio $HOME.
cd /home

14.-Verificar que se está en él.
pwd

15.-Listar todos los ficheros del directorio HOME mostrando su número de inodo.
ls -i

16.-Borrar todos los archivos y directorios visibles de vuestro directorio PRUEBA.
rm -rf PRUEBA/*

17.-Crear los directorios dir1, dir2 y dir3 en el directorio PRUEBA. Dentro de dir1 crear el directorio dir11.Dentro del directorio 
dir3 crear el directorio dir31. Dentro del directorio dir31, crear los directorios dir311 y dir312.


18.-Copiar el archivo /etc/motd a un archivo llamado mensaje de vuestro directorio PRUEBA.


19.-Copiar mensaje en dir1, dir2 y dir3.


20.-Comprobar el ejercicio anterior mediante un solo comando.


21.-Copiar los archivos del directorio rc.d que se encuentra en /etc al directorio dir31.


22.-Copiar en el directorio dir311 los archivos de /bin que tengan una a como segunda letra y su nombre tenga cuatro letras.

