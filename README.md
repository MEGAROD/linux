# Obligatorio - Taller de servidores linux

Este repositorio contiene los archivos y configuraciones necesarias para el despliegue de la aplicación "ToDo" mediante Ansible.

## Uso

1. Cambiar al directorio de los playbooks
```bash
cd /home/user/obligatorio/ansible/playbooks/
```
3. Desplegar App
```bash
ansible-playbook playbookcentos.yaml -i ../inventory/hosts --ask-become-pass
```
5. Desplegar DB
```bash
ansible-playbook playbookcentos.yaml -i ../inventory/hosts --ask-become-pass
```

# Detalles de los Playbooks

## APP

El playbook realiza las siguientes tareas:

1. Instalar JDK de Java
2. Crear usuario Tomcat
3. Crear grupo Tomcat
4. Descargar Tomcat
5. Crear directorio de instalación de Tomcat
6. Crear directorio de configuracion
7. Instalar unzip
8. Instalar tar
9. name: Extraer Tomcat
10. Cambiar permisos del directorio de Tomcat
11. Crear servicio systemD para Tomcat
12. Recargar systemD
13. Habilitar e iniciar Tomcat
14. Desplegar el archivo WAR
15. Copiar el archivo de configuración de la aplicación
16. Habilitar puertos en el firewall
17. Recargar el firewall

## DB

1. Configurar y asegurar MariaDB en Ubuntu
2. Configurar el intérprete de Python
3. Actualizar la lista de paquetes
5. Instalar MariaDB y herramientas relacionadas
6. Verificar si mysql_secure_installation está instalado
7. Mostrar ruta de mysql_secure_installation
8. Ejecutar mysql_secure_installation
