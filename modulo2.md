# ¿Qué es Ansible? 
Ansible es un software de gestión de la configuración automática y remota, que nos permite centralizar la configuración de numerosos servidores, dispositivos de red y Cloud Providers de una forma sencilla y automatizada.

## Términos y conceptos
Es necesario que se conozcan una serie de términos y sus usos:
-INVENTARIOS: Ansible trabaja, generalmente, ejecutando tareas contra distintos equipos remotos, dispositivos de red o APIs. Los inventarios, que pueden fijarse en formato Ansible INI, JSON o YAML, permiten definir dichos equipos, agruparlos y especificar valores grupales o individuales de estos.

-AD-HOC Commands: Un comando Ad-Hoc usa la herramienta de línea de comandos /usr/bin/ ansible para mecanizar una única tarea en uno o más nodos administrados. Estos comandos son rápidos y fáciles, pero no reutilizables, se utilizan en el momento.

-PLAYBOOKS: Estos son el lenguaje de configuración, implementación y orquestación de Ansible. Pueden describir la configuración que se desea que apliquen los equipos gestionados, o un conjuntos de fases en un proceso general de automatización.

-MÓDULOS: Se llaman también task plugins o library plugins, y son unidades discretas de código que se pueden usar desde la línea de comandos o en una tarea de Playbook. 

## RESUMEN
Tecnología de software libre que nos permite aprovisionar sistemas.

Mejoras significativas respecto a utilizar Shell scripts.

Amplia gama de módulos para aprovisionar servidores.

Herramienta declarativa.

Sin necesidad de configurar agentes.
