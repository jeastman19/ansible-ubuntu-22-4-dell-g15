<img src="images/dell-g15-5515-ryzen-edition.png" width="100px" alt="Dell G15 5515 Ryzen">
<img src="images/ansible-logo.png" width="100px">
<img src="images/ubuntu-logo14.png" width="100px">
<img src="images/docker.png" width="100px">
<img src="images/docker-compose-logo.png" width="100px">
<img src="images/Amazon_Web_Services_Logo.png" width="100px">
<img src="images/minikube-logo-mini.png" width="100px">
<img src="images/nvm.png" width="100px">
<img src="images/vsc.png" width="100px">
<img src="images/terraform.png" width="100px">
<img src="images/Slack.png" width="100px">

# Aprovicionamiento de equipo con Ubuntu 22.04 LTS utilizando Ansible

# Contenido

-   [Introducción](#introducción)
    -   [Requeriments](#requirementsyml)
    -   [Instalar Ansible](#instalar-ansible)
    -   [Roles externos](#roles-externos)

## Contenido de este proyecto

### requirements.yml

En este archivo están todos los Roles requeridos que serán instalados por Ansible previo a la ejecución del playbook.

Con el fin de facilitar la instalación de los roles, se ha creado un script denominado **_install-roles.sh_** que se encarga de descargar los roles requeridos, para ello se debe ejecutar:

```sh
./install-roles.sh
```

## Instalar Ansible

```sh
sudo apt install ansible
```

## Roles externos

Existen en [Ansible Galaxy][ansible galaxy] una gran cantidad de roles que nos permiten automatizar la instalación de software y configuraciones, en este proyecto hemos utilizado los siguientes:

-   [Git](https://galaxy.ansible.com/geerlingguy/git)
-   [Oh my zsh](https://galaxy.ansible.com/gantsign/oh-my-zsh)

# TODO

-   Probar: [ansible-galaxy install jonaspammer.bootstrap](https://galaxy.ansible.com/jonaspammer/bootstrap)

[ansible galaxy]: https://galaxy.ansible.com/
