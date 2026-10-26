
# Guía de comandos Linux

## 1. Sistema e información

| Comando | Descripción |
|---|---|
| `uname -a` | Información del sistema |
| `hostname` | Nombre del equipo |
| `uptime` | Tiempo encendido |
| `date` | Fecha y hora |
| `whoami` | Usuario actual |
| `id` | UID, GID y grupos |
| `who` | Usuarios conectados |
| `history` | Historial de comandos |
| `man comando` | Manual de un comando |
| `help` | Ayuda de Bash |
| `clear` | Limpia la terminal |
| `which comando` | Busca la ruta de un ejecutable |
| `whereis comando` | Busca binarios y manuales |

## 2. Archivos y directorios

| Comando | Descripción |
|---|---|
| `pwd` | Directorio actual |
| `ls` | Lista archivos |
| `ls -la` | Lista todos los archivos con detalles |
| `cd carpeta` | Cambia de directorio |
| `cd ..` | Sube un directorio |
| `cd ~` | Va al directorio personal |
| `mkdir carpeta` | Crea un directorio |
| `rmdir carpeta` | Elimina un directorio vacío |
| `touch archivo.txt` | Crea un archivo vacío |
| `cp origen destino` | Copia archivos |
| `cp -r origen destino` | Copia directorios |
| `mv origen destino` | Mueve o renombra archivos |
| `rm archivo` | Elimina un archivo |
| `rm -r carpeta` | Elimina una carpeta y su contenido |
| `file archivo` | Identifica el tipo de archivo |
| `stat archivo` | Muestra metadatos |
| `find /ruta -name "*.txt"` | Busca archivos |
| `locate archivo` | Busca archivos mediante una base de datos |
| `tree` | Muestra directorios en forma de árbol |
| `ln -s origen enlace` | Crea un enlace simbólico |
| `basename ruta` | Obtiene el nombre final de una ruta |
| `dirname ruta` | Obtiene el directorio de una ruta |

## 3. Lectura y edición de texto

| Comando | Descripción |
|---|---|
| `cat archivo` | Muestra el contenido |
| `tac archivo` | Muestra las líneas en orden inverso |
| `less archivo` | Lee un archivo por páginas |
| `more archivo` | Lectura paginada |
| `head archivo` | Muestra las primeras líneas |
| `tail archivo` | Muestra las últimas líneas |
| `tail -f archivo.log` | Sigue un registro en tiempo real |
| `nano archivo` | Edita texto |
| `vim archivo` | Editor de texto avanzado |
| `wc archivo` | Cuenta líneas, palabras y bytes |
| `wc -l archivo` | Cuenta líneas |
| `sort archivo` | Ordena líneas |
| `uniq archivo` | Filtra repeticiones consecutivas |
| `cut -d: -f1 archivo` | Extrae campos |
| `paste archivo1 archivo2` | Combina líneas de archivos |
| `tr 'a-z' 'A-Z'` | Convierte minúsculas en mayúsculas |
| `nl archivo` | Numera las líneas |
| `tee archivo` | Muestra y guarda una salida |
| `split archivo` | Divide archivos en partes |
| `diff archivo1 archivo2` | Compara archivos |

## 4. Búsqueda y filtros

| Comando | Descripción |
|---|---|
| `grep "texto" archivo` | Busca texto |
| `grep -i "texto" archivo` | Busca ignorando mayúsculas |
| `grep -r "texto" carpeta/` | Busca recursivamente |
| `sed 's/hola/adios/g' archivo` | Sustituye texto |
| `awk '{print $1}' archivo` | Extrae la primera columna |
| `xargs` | Convierte entradas en argumentos |
| `strings archivo` | Extrae cadenas legibles |
| `jq '.nombre' archivo.json` | Consulta datos JSON |

## 5. Usuarios y grupos

| Comando | Descripción |
|---|---|
| `whoami` | Muestra el usuario actual |
| `id` | Muestra UID, GID y grupos |
| `who` | Muestra usuarios conectados |
| `w` | Muestra usuarios y actividad |
| `su usuario` | Cambia de usuario |
| `sudo comando` | Ejecuta con privilegios autorizados |
| `passwd` | Cambia una contraseña |
| `useradd usuario` | Crea un usuario |
| `adduser usuario` | Asistente para crear usuarios |
| `usermod usuario` | Modifica un usuario |
| `userdel usuario` | Elimina un usuario |
| `groupadd grupo` | Crea un grupo |
| `groupmod grupo` | Modifica un grupo |
| `groupdel grupo` | Elimina un grupo |
| `groups usuario` | Muestra los grupos de un usuario |
| `getent passwd usuario` | Consulta información de usuario |
| `chage -l usuario` | Consulta la caducidad de contraseña |

## 6. Permisos y propietarios

| Comando | Descripción |
|---|---|
| `chmod 755 archivo` | Cambia permisos |
| `chmod 644 archivo` | Permite escritura al propietario y lectura a todos |
| `chmod 700 carpeta` | Permisos completos solo para el propietario |
| `chown usuario archivo` | Cambia el propietario |
| `chown usuario:grupo archivo` | Cambia propietario y grupo |
| `chgrp grupo archivo` | Cambia el grupo propietario |
| `umask` | Consulta la máscara de permisos |
| `getfacl archivo` | Consulta permisos ACL |
| `setfacl` | Configura permisos ACL |
| `ls -l` | Muestra permisos y propietarios |

## 7. Procesos y rendimiento

| Comando | Descripción |
|---|---|
| `ps aux` | Lista procesos |
| `top` | Monitoriza procesos |
| `htop` | Monitor interactivo |
| `pgrep nombre` | Busca procesos por nombre |
| `pidof programa` | Obtiene el PID de un programa |
| `pstree` | Muestra procesos en forma de árbol |
| `kill PID` | Envía una señal a un proceso |
| `killall programa` | Envía una señal por nombre |
| `pkill nombre` | Busca procesos y les envía una señal |
| `nice comando` | Inicia un proceso con prioridad determinada |
| `renice prioridad -p PID` | Cambia la prioridad |
| `jobs` | Lista trabajos de la terminal |
| `bg` | Continúa un trabajo en segundo plano |
| `fg` | Trae un trabajo al primer plano |
| `nohup comando &` | Ejecuta un comando independiente de la terminal |
| `free -h` | Muestra el uso de memoria |
| `vmstat` | Estadísticas de memoria y procesos |
| `lscpu` | Información de CPU |
| `watch comando` | Repite un comando periódicamente |
| `time comando` | Mide la duración de un comando |

## 8. Discos y almacenamiento

| Comando | Descripción |
|---|---|
| `lsblk` | Lista discos y particiones |
| `blkid` | Muestra identificadores de dispositivos |
| `fdisk -l` | Consulta las particiones |
| `parted -l` | Consulta tablas de particiones |
| `mkfs` | Crea un sistema de archivos |
| `fsck` | Comprueba sistemas de archivos compatibles |
| `mount` | Monta sistemas de archivos |
| `umount` | Desmonta sistemas de archivos |
| `findmnt` | Muestra sistemas montados |
| `df -h` | Muestra espacio libre y ocupado |
| `du -sh carpeta` | Calcula el espacio ocupado |
| `dd` | Copia datos a bajo nivel |
| `smartctl` | Consulta información SMART |
| `fstrim` | Solicita liberar bloques no utilizados |
| `swapon --show` | Muestra el espacio de intercambio |
| `swapoff` | Desactiva espacio de intercambio |

**Precaución:** `rm -r`, `mkfs`, `fdisk` y `dd` pueden provocar pérdida de datos si se usan incorrectamente.

## 9. Redes y conectividad

| Comando | Descripción |
|---|---|
| `ip addr` | Muestra direcciones IP |
| `ip link` | Muestra interfaces de red |
| `ip route` | Muestra la tabla de rutas |
| `ping -c 4 8.8.8.8` | Comprueba conectividad |
| `tracepath dominio` | Examina la ruta hacia un destino |
| `traceroute dominio` | Muestra los saltos de red |
| `mtr dominio` | Diagnostica ruta y latencia |
| `ss -tuln` | Muestra puertos y sockets |
| `netstat -tuln` | Consulta puertos con la herramienta tradicional |
| `dig dominio` | Consulta DNS |
| `nslookup dominio` | Consulta DNS |
| `host dominio` | Consulta DNS sencilla |
| `resolvectl status` | Consulta la configuración DNS |
| `curl -I URL` | Consulta cabeceras HTTP |
| `wget URL` | Descarga archivos |
| `ssh usuario@servidor` | Conecta remotamente por SSH |
| `scp archivo usuario@servidor:/ruta` | Copia archivos por SSH |
| `sftp usuario@servidor` | Transfiere archivos mediante SFTP |
| `rsync -av origen/ destino/` | Sincroniza archivos |
| `nc -vz servidor 22` | Comprueba una conexión a un puerto |
| `nmcli device status` | Consulta dispositivos de red |
| `nmtui` | Configura la red de forma interactiva |
| `ethtool interfaz` | Consulta parámetros Ethernet |
| `iw dev` | Consulta interfaces inalámbricas |
| `tcpdump -i interfaz` | Captura paquetes de red |
| `hostname -I` | Muestra las direcciones IP locales |

## 10. Gestión de paquetes

### Debian, Ubuntu y Kali Linux

| Comando | Descripción |
|---|---|
| `sudo apt update` | Actualiza los índices de paquetes |
| `sudo apt upgrade` | Actualiza paquetes instalados |
| `sudo apt full-upgrade` | Actualiza paquetes gestionando dependencias |
| `sudo apt install paquete` | Instala un paquete |
| `sudo apt remove paquete` | Desinstala un paquete |
| `sudo apt purge paquete` | Desinstala y elimina su configuración gestionada |
| `sudo apt autoremove` | Elimina dependencias innecesarias |
| `apt search texto` | Busca paquetes |
| `apt show paquete` | Muestra información |
| `apt list --installed` | Lista paquetes instalados |
| `dpkg -i archivo.deb` | Instala un paquete DEB local |
| `dpkg -l` | Lista paquetes conocidos por dpkg |
| `dpkg -L paquete` | Lista archivos instalados por un paquete |

### Fedora y distribuciones relacionadas

| Comando | Descripción |
|---|---|
| `sudo dnf install paquete` | Instala un paquete |
| `sudo dnf upgrade` | Actualiza paquetes |
| `sudo dnf remove paquete` | Desinstala un paquete |
| `dnf search texto` | Busca paquetes |
| `rpm -qa` | Lista paquetes RPM instalados |
| `rpm -qi paquete` | Muestra información de un paquete |

### Arch Linux

| Comando | Descripción |
|---|---|
| `sudo pacman -S paquete` | Instala un paquete |
| `sudo pacman -Syu` | Actualiza el sistema |
| `sudo pacman -R paquete` | Desinstala un paquete |
| `pacman -Ss texto` | Busca paquetes |
| `pacman -Q` | Lista paquetes instalados |
| `pacman -Qi paquete` | Muestra información de un paquete |

## 11. Servicios y registros

| Comando | Descripción |
|---|---|
| `systemctl status servicio` | Consulta el estado de un servicio |
| `sudo systemctl start servicio` | Inicia un servicio |
| `sudo systemctl stop servicio` | Detiene un servicio |
| `sudo systemctl restart servicio` | Reinicia un servicio |
| `sudo systemctl reload servicio` | Recarga su configuración |
| `sudo systemctl enable servicio` | Habilita el inicio automático |
| `sudo systemctl disable servicio` | Deshabilita el inicio automático |
| `systemctl list-units` | Lista unidades cargadas |
| `systemctl --failed` | Muestra unidades fallidas |
| `systemd-analyze` | Analiza el arranque |
| `journalctl` | Consulta registros del sistema |
| `journalctl -b` | Consulta registros del arranque actual |
| `journalctl -u servicio` | Consulta registros de un servicio |
| `dmesg` | Muestra mensajes del kernel |
| `lsmod` | Lista módulos cargados |
| `modinfo modulo` | Muestra información de un módulo |
| `sudo modprobe modulo` | Carga un módulo compatible |
| `sudo rmmod modulo` | Retira un módulo cargado |

## 12. Apagado y reinicio

| Comando | Descripción |
|---|---|
| `sudo shutdown -h now` | Apaga el equipo |
| `sudo shutdown -r now` | Reinicia el equipo |
| `sudo shutdown +10` | Programa el apagado en 10 minutos |
| `sudo shutdown -c` | Cancela un apagado programado |
| `reboot` | Reinicia el sistema |
| `poweroff` | Apaga el sistema |
| `systemctl suspend` | Suspende el sistema |
| `systemctl hibernate` | Hiberna el sistema si está configurado |
| `loginctl` | Consulta y gestiona sesiones |
| `exit` | Sale de la shell actual |

## 13. Compresión y copias de seguridad

| Comando | Descripción |
|---|---|
| `tar -cvf copia.tar carpeta/` | Crea un archivo TAR |
| `tar -czf copia.tar.gz carpeta/` | Crea un TAR comprimido con gzip |
| `tar -xzf copia.tar.gz` | Extrae un TAR comprimido |
| `gzip archivo` | Comprime un archivo |
| `gunzip archivo.gz` | Descomprime gzip |
| `bzip2 archivo` | Comprime con bzip2 |
| `bunzip2 archivo.bz2` | Descomprime bzip2 |
| `xz archivo` | Comprime con xz |
| `unxz archivo.xz` | Descomprime xz |
| `zip -r copia.zip carpeta/` | Crea un ZIP |
| `unzip copia.zip` | Extrae un ZIP |
| `7z a copia.7z carpeta/` | Crea un archivo 7z |
| `zstd archivo` | Comprime con Zstandard |
| `sha256sum archivo` | Calcula un hash SHA-256 |
| `md5sum archivo` | Calcula un hash MD5 |

## 14. Variables y entorno

| Comando | Descripción |
|---|---|
| `echo "Hola"` | Imprime texto |
| `printf` | Imprime texto con formato |
| `env` | Muestra el entorno |
| `printenv PATH` | Muestra una variable |
| `export VARIABLE=valor` | Exporta una variable |
| `unset VARIABLE` | Elimina una variable |
| `alias ll='ls -la'` | Crea un alias |
| `unalias ll` | Elimina un alias |
| `set -o` | Consulta opciones de shell |
| `source ~/.bashrc` | Ejecuta la configuración de Bash |
| `exec comando` | Sustituye el proceso actual por otro |
| `sleep 5` | Espera cinco segundos |
| `seq 1 10` | Genera números del 1 al 10 |
| `xargs` | Construye argumentos a partir de una entrada |

## 15. Redirecciones y operadores

| Símbolo | Descripción | Ejemplo |
|---|---|---|
| `>` | Escribe y reemplaza el archivo | `ls > lista.txt` |
| `>>` | Añade al final del archivo | `date >> registro.txt` |
| `<` | Redirige la entrada | `sort < nombres.txt` |
| `\|` | Conecta la salida de un comando con otro | `ls \| grep txt` |
| `2>` | Redirige los errores | `comando 2> errores.log` |
| `2>&1` | Envía los errores al destino de la salida estándar | `comando > salida.log 2>&1` |
| `&&` | Ejecuta el siguiente comando si el anterior tiene éxito | `mkdir prueba && cd prueba` |
| `\|\|` | Ejecuta el siguiente comando si el anterior falla | `comando \|\| echo Error` |
| `;` | Ejecuta comandos consecutivamente | `pwd; ls` |
| `&` | Ejecuta un comando en segundo plano | `sleep 30 &` |
| `*` | Coincide con varios caracteres en nombres | `ls *.txt` |
| `?` | Coincide con un carácter en nombres | `ls archivo?.txt` |
| `$VAR` | Expande una variable | `echo "$HOME"` |
| `$(...)` | Sustituye un comando por su salida | `echo "$(date)"` |

## 16. Scripts Bash

| Elemento | Descripción |
|---|---|
| `bash script.sh` | Ejecuta un script |
| `read -r variable` | Lee una entrada |
| `if` | Evalúa una condición |
| `case` | Selecciona entre opciones |
| `for` | Repite instrucciones |
| `while` | Repite mientras se cumpla una condición |
| `function` | Define una función |
| `return` | Devuelve un estado desde una función |
| `exit` | Finaliza el script |
| `break` | Sale de un bucle |
| `continue` | Pasa a la siguiente iteración |
| `trap` | Gestiona señales y eventos |
| `set -e` | Sale ante determinados errores no controlados |
| `set -x` | Muestra los comandos ejecutados |
| `crontab -e` | Edita tareas periódicas |
| `crontab -l` | Lista tareas programadas |

### Ejemplo de script

```bash
#!/bin/bash

echo "¿Cómo te llamas?"
read -r nombre
echo "Hola, $nombre"

exit 0
```

Ejecutar:

```bash
bash saludo.sh
```

## 17. Fecha y tareas programadas

| Comando | Descripción |
|---|---|
| `date` | Muestra fecha y hora |
| `timedatectl` | Consulta la configuración horaria |
| `cal` | Muestra un calendario, si está instalado |
| `sleep 10` | Espera 10 segundos |
| `watch comando` | Repite un comando |
| `crontab -e` | Edita tareas periódicas |
| `crontab -l` | Lista tareas programadas |
| `atq` | Lista trabajos pendientes de at |
| `atrm trabajo` | Elimina un trabajo programado |
| `timeout 10 comando` | Limita la duración de un comando |

## 18. Hardware

| Comando | Descripción |
|---|---|
| `lscpu` | Información del procesador |
| `lspci` | Dispositivos PCI |
| `lsusb` | Dispositivos USB |
| `lsblk` | Discos y particiones |
| `lshw` | Inventario de hardware |
| `dmidecode` | Información DMI/SMBIOS |
| `free -h` | Uso de memoria |
| `sensors` | Sensores y temperaturas |
| `inxi` | Resumen del hardware |
| `lsmod` | Módulos del kernel |
| `dmesg` | Mensajes del kernel |
| `udevadm` | Información de dispositivos |
| `lsof` | Archivos abiertos por procesos |
| `cat /proc/cpuinfo` | Información de CPU |
| `cat /proc/meminfo` | Información de memoria |

## 19. Seguridad

| Comando | Descripción |
|---|---|
| `ssh-keygen` | Genera claves SSH |
| `ssh-agent` | Gestiona claves SSH en memoria |
| `ssh-add` | Añade claves al agente SSH |
| `gpg` | Cifra, descifra y firma datos |
| `openssl` | Herramientas criptográficas |
| `sha256sum archivo` | Calcula un hash SHA-256 |
| `sha512sum archivo` | Calcula un hash SHA-512 |
| `sudo -l` | Muestra privilegios sudo disponibles |
| `ufw status` | Consulta el estado del cortafuegos UFW |
| `nft list ruleset` | Consulta reglas nftables |
| `iptables -L` | Consulta reglas de iptables |
| `getfacl archivo` | Consulta permisos ACL |

## 20. Usuarios conectados y registros

| Comando | Descripción |
|---|---|
| `who` | Muestra usuarios conectados |
| `w` | Muestra usuarios y actividad |
| `last` | Historial de inicios de sesión |
| `lastlog` | Último inicio de sesión por usuario |
| `journalctl` | Registros del sistema |
| `dmesg` | Mensajes del kernel |
| `logger "mensaje"` | Envía un mensaje al registro |
| `tail -f archivo.log` | Sigue un registro en tiempo real |
| `logrotate` | Gestiona la rotación de registros |
| `systemctl --failed` | Muestra unidades fallidas |

## 21. Impresión y dispositivos

| Comando | Descripción |
|---|---|
| `lp archivo` | Envía un archivo a imprimir |
| `lpstat` | Consulta el estado de impresión |
| `cancel trabajo` | Cancela un trabajo de impresión |
| `lpq` | Consulta la cola de impresión |
| `lpr archivo` | Envía un archivo a imprimir |
| `lsusb` | Lista dispositivos USB |
| `udevadm` | Consulta información de dispositivos |
| `bluetoothctl` | Gestiona Bluetooth |
| `rfkill` | Consulta bloqueos de radio |
| `lsblk` | Lista dispositivos de bloques |

## 22. Desarrollo y compilación

| Comando | Descripción |
|---|---|
| `git` | Control de versiones |
| `python3` | Ejecuta Python |
| `pip` | Gestiona paquetes Python |
| `gcc` | Compila programas C |
| `g++` | Compila programas C++ |
| `make` | Automatiza compilaciones |
| `cmake` | Configura proyectos de compilación |
| `node` | Ejecuta JavaScript con Node.js |
| `npm` | Gestiona paquetes Node.js |
| `php` | Ejecuta PHP |
| `ruby` | Ejecuta Ruby |
| `perl` | Ejecuta Perl |
| `java` | Ejecuta aplicaciones Java |
| `javac` | Compila Java |
| `go` | Herramientas de Go |
| `rustc` | Compila Rust |
| `cargo` | Gestiona proyectos Rust |
| `docker` | Gestiona contenedores Docker |
| `podman` | Gestiona contenedores Podman |

## 23. Contenedores y virtualización

| Comando | Descripción |
|---|---|
| `docker ps` | Lista contenedores en ejecución |
| `docker images` | Lista imágenes |
| `docker pull imagen` | Descarga una imagen |
| `docker run imagen` | Inicia un contenedor |
| `docker stop contenedor` | Detiene un contenedor |
| `docker start contenedor` | Inicia un contenedor existente |
| `docker logs contenedor` | Muestra registros |
| `docker exec contenedor comando` | Ejecuta un comando en un contenedor |
| `podman ps` | Lista contenedores Podman |
| `virsh list --all` | Lista máquinas virtuales de libvirt |
| `VBoxManage` | Gestiona VirtualBox desde la terminal |

## 24. Atajos de teclado

| Atajo | Función |
|---|---|
| `Ctrl + C` | Interrumpe un proceso en primer plano |
| `Ctrl + Z` | Suspende un proceso en primer plano |
| `Ctrl + D` | Envía fin de entrada |
| `Ctrl + L` | Limpia visualmente la terminal |
| `Ctrl + A` | Va al principio de la línea |
| `Ctrl + E` | Va al final de la línea |
| `Ctrl + U` | Borra hasta el principio de la línea |
| `Ctrl + K` | Borra hasta el final de la línea |
| `Ctrl + W` | Borra la palabra anterior |
| `Tab` | Completa comandos y nombres |
| `Flecha arriba` | Recupera el comando anterior |
| `Flecha abajo` | Avanza por el historial |
| `Ctrl + R` | Busca en el historial |

## 25. Descubrir comandos disponibles

```bash
# Mostrar las rutas de búsqueda de ejecutables
echo "$PATH"

# Listar comandos conocidos por Bash
compgen -c | sort -u

# Consultar la ayuda de Bash
help

# Buscar la ruta de un ejecutable
which ls

# Buscar páginas de manual por tema
man -k .

# Listar paquetes en Debian y Ubuntu
dpkg -l

# Listar paquetes en Fedora
rpm -qa

# Listar paquetes en Arch Linux
pacman -Q
```

## 26. Comandos más importantes para SMX

| Comando | Uso principal |
|---|---|
| `ls` | Listar archivos |
| `cd` | Cambiar de directorio |
| `pwd` | Consultar la ruta actual |
| `mkdir` | Crear carpetas |
| `cp` | Copiar archivos |
| `mv` | Mover o renombrar |
| `rm` | Eliminar archivos |
| `cat` | Leer archivos |
| `grep` | Buscar texto |
| `find` | Buscar archivos |
| `chmod` | Cambiar permisos |
| `chown` | Cambiar propietarios |
| `sudo` | Ejecutar con privilegios |
| `ps` | Consultar procesos |
| `kill` | Enviar señales a procesos |
| `ip` | Consultar configuración de red |
| `ping` | Comprobar conectividad |
| `ssh` | Conectar a equipos remotos |
| `apt` | Gestionar paquetes en Debian/Ubuntu |
| `systemctl` | Gestionar servicios |

---

**Nota:** esta guía reúne comandos comunes, pero no incluye absolutamente todas las herramientas existentes en Linux. Algunos comandos requieren instalación adicional, permisos de administrador o una distribución específica. Antes de ejecutar comandos que modifiquen discos, permisos o archivos, comprueba sus efectos.
