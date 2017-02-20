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

mkdir PRUEBA

mkdir PRUEBA/dir1

mkdir PRUEBA/dir1/dir11

mkdir PRUEBA/dir2

mkdir PRUEBA/dir3

mkdir PRUEBA/dir3/dir31

mkdir PRUEBA/dir3/dir31/dir311

18.-Copiar el archivo /etc/motd a un archivo llamado mensaje de vuestro directorio PRUEBA.

cp /etc/moth PRUEBA/mensaje


19.-Copiar mensaje en dir1, dir2 y dir3.

cp PRUEBA/mensaje PRUEBA/dir1
cp PRUEBA/mensaje PRUEBA/dir2
cp PRUEBA/mensaje PRUEBA/dir3

20.-Comprobar el ejercicio anterior mediante un solo comando.

tree

21.-Copiar los archivos del directorio rc0.d que se encuentra en /etc al directorio dir31.

cp /etc/rc0.d/* PRUEBA/dir3/dir31/ 


22.-Copiar en el directorio dir311 los archivos de /bin que tengan una a como segunda letra y su nombre tenga cuatro letras.

cp /bin/?a?? PRUEBA/dir3/dir31/dir311

23.-Copiar el directorio de otro usuario y sus subdirectorios debajo de dir11 (incluido el propio directorio).

24.-Mover el directorio dir31 y sus subdirectorios debajo de dir2.

mv PRUEBA/dir3/dir31 PRUEBA/dir2

25.-Mostrar por pantalla los archivos ordinarios del directorio HOME y sus subdirectorios.

tree /home |more

26.-Ocultar el archivo mensaje del directorio dir3.

mv PRUEBA/dir3/mensaje PRUEBA/dir3/.mensaje

27.-Borrar los archivos y directorios de dir1, incluido el propio directorio.

rm -rf PRUEBA/dir1

28.-Copiar al directorio dir312 los ficheros del directorio /dev que empiecen por t, acaben en una letra que vaya de la a a la b y tengan cinco letras en su nombre.

ls /dev/t????[a*b]

29.-Borrar los archivos de dir312 que no acaben en b y tengan una q como cuarta letra.

rm PRUEBA/dir2/dir31/dir312/???q*[^b]

30.-Mover el directorio dir312 debajo de dir3.

mv PRUEBA/dir2/dir31/dir312 PRUEBA/dir3

31.-Crear un enlace simbólico al directorio dir1 dentro del directorio dir3 llamado enlacedir1.

ln -s /home/marta/PRUEBA/dir1 PRUEBA/dir3/enlacedir1

32.-Posicionarse en dir3 y, empleando el enlace creado en el ejercicio anterior, crear el directorio nuevo1 dentro de dir1.

cd PRUEBA/dir3

mkdir enlacedir1/nuevo1

33.-Utilizando el enlace creado copiar los archivos que empiecen por u del directorio /bin en directorio nuevo1.

cp /bin/u* enlacedir1/nuevo1/

34.-Crear dos enlaces duros del fichero fich1, llamarlo enlace, en los directorios dir1 y dir2.

igual que el otro de crear enlaces pero sin el -s

35.-Borrar el archivo fich1 y copiar enlace en dir3.


36.-Crear un enlace simbólico (llamado enlafich1) al fichero enlace de dir2 en dir1.


37.-Posicionarse en dir1 y, mediante el enlace creado, copiar el archivo fichl dentro de dir311.


38.-Seguir en dir1 y, mediante el enlace creado, sacar por pantalla las líneas que tiene el archivo fich1.


39.-Borrar el fichero fich1 de dir2.


40.-Borrar todos los archivos y directorios creados durante los ejercicios.


41.-Crear el directorio dir2 y dir3 en el directorio PRUEBA ¿Cuáles son los actuales permisos del directorio dir2?


42.-Utilizando la notación simbólica, eliminar todos los permisos de escritura (propietario, grupo, otros) del directorio dir2.
chmod u +r - w (ta mal)

43.-Utilizando la notación octal, eliminar el permiso de lectura del directorio dir2, al resto de los usuarios.


44.-¿Cuáles son ahora los permisos asociados a dir2?


45.-Crear bajo dir2, un directorio llamado dir2l.


46.-Concederse a sí mismo permiso de escritura en el directorio dir2 e intentar de nuevo el paso anterior.


47.-¿Cuáles son los valores por omisión asignados a los archivos?


48.-Cambiar el directorio actual al directorio dir3. Imprimir su trayectoria completa para verificar el cambio.


49.-¿Cuáles son los permisos asignados en su momento a este directorio?


50.-Reiniciar el ordenador.

