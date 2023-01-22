# Configurar un playbook en Ansible.

Un Playbook en Ansible hace referencia a cada uno de los scripts que monta el usuario, es decir, un fichero que describe el paso a paso a ejecutar en una máquina determinada y que se usa para un objetivo específico o como plantilla que marca la hoja de ruta durante el inicio de un determinado proyecto. 

Un Playbook está formado por uno o más play, que son los pasos a realizar y que pueden incluir una o más tareas, que se realizan de manera ordenada y solo una al mismo tiempo. Es importante mantener el orden correcto de estas tareas, ya que el Playbook se ejecutará de forma secuencial y seguirá la disposición determinada por el usuario.

### Creación de fichero hosts
Este fichero contiene información sobre los hosts que va a administrar Ansible. Como yo solo tengo un cliente creo el archivo y le añado su IP como se ve a continuación.

![hosts](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20PLAYBOOK/1.PNG?raw=true)

### Creación de Playbook

Para crear un playbook debemos saber que está escrita en un lenguaje de texto plano, en el formato de serialización de datos YAML, que facilita la legibilidad y la capacidad de escritura del usuario de Ansible. El uso del lenguaje YAML trae como resultado que un Playbook en Ansible necesite empezar con tres guiones (- – – ) y que requiera el uso de una sangría adecuada que funcione a través de espacios y no de tabuladores.

Vamos a crear uno. Primero creo el fichero .yaml en la misma carpeta donde he creado el de hosts. 

![playbook](https://github.com/samarameit/Ansible/blob/main/ANSIBLE%20PLAYBOOK/4.PNG?raw=true)

Lo primero que vemos es una declaración de tipo hosts, que se encargará de señalar en qué servidor se llevará a cabo el proceso. Indicamos que es webserver ya que es el nombre que le hemos puesto dentro del fichero de hosts. En remote_user ponemos el usuario que hemos creado en la máquina cliente. Después de esto, en tasks establecemos las tareas que queremos ejecutar en orden. En mi caso he puesto dos tareas. Primero quiero instalar la última versión de Apache en caso de que no esté instalada, y en segundo lugar quiro que el servicio esté activo. Con become indicamos que tiene que tener permisos de sudo para realizar las tareas.

El siguiente paso sería desplegar los servicios con Ansible ->
[Desplegar Servicios](https://github.com/samarameit/Ansible/blob/main/modulo5.md)
