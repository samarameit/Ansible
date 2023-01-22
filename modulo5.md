# Desplegar servicios en Ansible

Para desplegar los servicios de esta herramienta se debe ejecutar el comando ansible-playbook en el nodo de control (máquina servidor) seguido del nombre de archivo .yml donde se encuentra el código a ejecutar. Ponemos --ask-become-pass en el comando para que nos pida la contraseña del cliente. 

![desplegar](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20PLAYBOOK/5.PNG?raw=true)

Vemos que ha conectado correctamente con el cliente y ha realizado las tareas indicadas. Si hubiese algún fallo saldría en rojo en FAILED. 
