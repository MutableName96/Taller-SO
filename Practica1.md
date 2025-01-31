<div align="center">
<h1>PRACTICA 1</h1> 
<h3>Nombre: Antonio López Martínez</h3>  
<h3>Numero Control: 22121322</h3>  
<h3>Maestra: Brenda</h3> 
<img src="OIP.jpeg" alt="Portada"></img> 
</div>



---

#### | ls
```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ ls
archivo1.txt  backup         contraseñas_cifrado.txt     contraseñas.txt  dispositivos.sh  Escritorio  listado.txt  Plantillas   Público                  snap
archivo2.txt  backup.tar.gz  contraseñas_descifrado.txt  Descargas        Documentos       Imágenes    Música       privado.txt  resumendispositivos.txt  Vídeos
```
|  Capa de Hardware | Nuleo  | Espacio de Usuario  |
|:---------:|:---------:|:---------:|
| ✅| ✅| 🟥|


Al solo mostrar los archivos accede a la parte del administrador de archivos que seria la parte del nucleo y al hardware porque tiene que consultar lo que hay en disco para mostrarlo y no estoy seguro si la consola podria entrar como parte de usuario puede que si o no pero lo tomare mejor como que no porque no lo considero como una aplicacion como tal sino como algo escencial del SO, pero si se considera como app pues en todos los comandos se podria decir que si se usa el espacio de usuario


#### | ls -l
```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ ls -l
total 100
-rw-rw-r-- 1 mutablename96 mutablename96    29 dic 15 18:59 archivo1.txt
-rw-rw-r-- 1 mutablename96 mutablename96    29 dic 15 18:59 archivo2.txt
drwxrwxr-x 2 mutablename96 mutablename96  4096 dic 15 20:13 backup
-rw-rw-r-- 1 mutablename96 mutablename96   522 dic 15 20:13 backup.tar.gz
-rw-rw-r-- 1 mutablename96 mutablename96    48 dic 18 19:50 contraseñas_cifrado.txt
-rw-rw-r-- 1 mutablename96 mutablename96    30 dic 18 19:55 contraseñas_descifrado.txt
-rw-rw-r-- 1 mutablename96 mutablename96    30 dic 18 19:50 contraseñas.txt
drwxr-xr-x 3 mutablename96 mutablename96  4096 ene 30 11:42 Descargas
-rwxrwxr-x 1 mutablename96 mutablename96  1052 dic 15 15:22 dispositivos.sh
drwxr-xr-x 5 mutablename96 mutablename96  4096 ene 30 11:35 Documentos
drwxr-xr-x 2 mutablename96 mutablename96  4096 dic 15 17:04 Escritorio
drwxr-xr-x 3 mutablename96 mutablename96  4096 dic 17 17:01 Imágenes
-rw-rw-r-- 1 mutablename96 mutablename96  1111 dic 15 18:54 listado.txt
drwxr-xr-x 2 mutablename96 mutablename96  4096 nov  1 18:26 Música
drwxr-xr-x 2 mutablename96 mutablename96  4096 nov  1 18:26 Plantillas
-rw------- 1 pepe          mutablename96     0 dic 15 21:15 privado.txt
drwxr-xr-x 2 mutablename96 mutablename96  4096 nov  1 18:26 Público
-rw-rw-r-- 1 mutablename96 mutablename96 26770 dic 15 15:25 resumendispositivos.txt
drwx------ 8 mutablename96 mutablename96  4096 dic  1 19:39 snap
drwxr-xr-x 2 mutablename96 mutablename96  4096 nov  1 18:26 Vídeos

```
|  Capa de Hardware | Nuleo  | Espacio de Usuario  |
|:---------:|:---------:|:---------:|
| ✅ | ✅| 🟥|

Esto es lo mismo que el anterior lo que cambia es que al usar eel -l muestra mas detalles de los archivos pero sigue siguiendo el mismo proceso pero con informacion extra 
#### | ls -a
```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ ls -a
.             backup         .bashrc                  contraseñas_descifrado.txt  Documentos  .gnupg       .local      privado.txt              snap                       .vscode
..            backup.tar.gz  .cache                   contraseñas.txt             .dotnet     Imágenes     Música      .profile                 .ssh
archivo1.txt  .bash_history  .config                  Descargas                   Escritorio  .lesshst     .pki        Público                  .sudo_as_admin_successful
archivo2.txt  .bash_logout   contraseñas_cifrado.txt  dispositivos.sh             .gitconfig  listado.txt  Plantillas  resumendispositivos.txt  Vídeos

```

|  Capa de Hardware | Nuleo  | Espacio de Usuario  |
|:---------:|:---------:|:---------:|
| ✅ | ✅| 🟥|

Este comando es casi lo mismo que el ls solo que al usar el -a se pueden mostrar archivos que puedan estar ocultos pero sigue usando el mismo proceso de consultar el disco para mostrarlo a travez del nucle 


#### | cat /proc/cpuinfo
```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ cat /proc/cpuinfo
processor	: 0
vendor_id	: GenuineIntel
cpu family	: 6
model		: 158
model name	: Intel(R) Core(TM) i7-9750H CPU @ 2.60GHz
stepping	: 10
microcode	: 0xf8
cpu MHz		: 800.031
cache size	: 12288 KB
physical id	: 0
siblings	: 12
core id		: 0
cpu cores	: 6
apicid		: 0
initial apicid	: 0
fpu		: yes
fpu_exception	: yes
cpuid level	: 22
wp		: yes

```

|  Capa de Hardware | Nuleo  | Espacio de Usuario  |
|:---------:|:---------:|:---------:|
| ✅ | ✅| 🟥|

Este comando consulta la informacion del procesador de los drivers que nos muestra como el nombre, cantidad de nucleos velocidad, el vendedor etc... es la misma logica que los anteriores esa informacion generalmente se almacena en el kernel de linux asi que en algun momento tuvo que haber interactuado con la capa de hardware para saberlo incluso usando la BIOS

#### | free -h
`-h` Muestra los datos en un formato que pueda leerse es decir en MB o GB.

`free -m` Muestra los valores en megabytes

```bash
mutablename96@mutablename96-Nitro-AN515-54:~$ free -h
               total       usado       libre  compartido   búf/caché  disponible
Mem:            15Gi       4,0Gi       8,9Gi       567Mi       3,4Gi        11Gi
Inter:         4,0Gi          0B       4,0Gi
```

|  Capa de Hardware | Nuleo  | Espacio de Usuario  |
|:---------:|:---------:|:---------:|
| ✅ | ✅| 🟥|

Este comando nos muestra inforamcion acerca de nuestra ram y de la memoria swap y podemos decir que interactua con las capas de hardware y nucleo ya que se consulta el espacio fisico de la ram y tambien el swap al usar el concepto de memoria virtual para ir liberando la ram tambien hace uso del nucleo de muchas formas