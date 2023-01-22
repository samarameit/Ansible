# Instalación de Ansible

Lo primero que vamos a necesitar para la instalación de Ansible será un nodo de control Ansible y uno o más hosts de Ansible (cualquier máquina en la que su nodo de control de ansible este configurado para la automatización). Voy a usar dos máquinas Debian. Ambas deben estar configuradas en la misma red.

### Instalación

1. Antes de nada en la máquina servidor donde vamos a instalar Ansible uso el comando 'apt update' siendo root.

![update](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20INSTALACION/1.PNG?raw=true)

2. Instalamos Ansible desde los repositorios.

![instalacion](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20INSTALACION/2.PNG?raw=true)

Ya lo tendríamos instalado.

### Preparativos

Además de la instalación vamos a necesitar poder conectarnos por ssh entre la máquina servidor y la máquina cliente de forma automatizada. Primero creamos en el cliente un nuevo usuario para no tener que conectarnos con root, en este caso creo mi usuario Samara y le doy permisos de root con el comando 'usermod -aG sudo samara'. 

![usuario](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20INSTALACION/3.PNG?raw=true)

![permisos](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20INSTALACION/4.PNG?raw=true)

Ahora en la maquina servidor utilizamos el comando ssh-keygen para crear la clave ssh. Despues mandamos la clave al cliente. Mandamos la clave al usuario que acabamos de crear.

![ssh-keygen](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20INSTALACION/5.PNG?raw=true)

![ssh](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20INSTALACION/6.PNG?raw=true)

Ya tenemos todo listo para el siguiente paso -> [Configurar Playbook](https://github.com/samarameit/Ansible/blob/main/modulo4.md)
