
﻿## Este repositorio busca implemtar un LEMP en Centos 10 Stream con Ansible

 https://www.digitalocean.com/community/tutorials/how-to-install-linux-nginx-mysql-php-lemp-stack-on-centos-7

 Prerequisitos descagar vagrant --> https://developer.hashicorp.com/vagrant/install

 Este `README` proporciona instrucciones básicas para la instalación de herramientas necesarias y la configuración de una máquina virtual con Vagrant con las herramientas necesarias.

## Configuración de Vagrant :

En el directorio de tu proyecto, encontrarás una carpeta llamada "Vagrant". Esta carpeta contiene la configuración necesaria para levantar una máquina virtual.

1. **Iniciar la Máquina Virtual**: Ejecuta el siguiente comando dentro del directorio "Vagrant":
   ```bash
   vagrant up
   ```
2. **Conexión SSH**:  Para conectarte a la máquina virtual por SSH, utiliza el siguiente comando:
   ```bash
   vagrant ssh
   ```

## Dentro de Vagrant :

1. **Dentro de la VM**: Ejecuta los siguientes comando para instalar Ansible:
   ```bash
   cd /vagrant
   ```
   ```bash
   ./InstalarAnsible.sh
   ```
   
2. **Correr Playbook**:  Correr el playbook para desplegar el LEMP:
   ```bash
   ansible-playbook playbook.yml
   ```

3. **Averiguar IP**:  Podes verificar la correcta instalacion con la IP:
   ```bash
   hostname -I
   ```
4- **Ingresar IP** Ingresar la ip del host en el buscador para ver el nginx y el php
   ```bash
   nginx --> http://server_domain_name_or_IP/
   ```
   ```bash
   PHP   --> http://server_host_or_IP/info.php
   ```   
    
    
