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

-   [Objetivo](#objetivo)
    -   [Instalar Ansible](#instalar-ansible)
    -   [Roles externos](#roles-externos)
-   [Anexos](#anexos)
    -   [Roles externos](#roles-externos-1)

## Objetivo

El objetivo de este proyecto es automatizar la instalación de software y configuraciones en un equipo con Ubuntu 22.04 LTS, para ello se ha utilizado Ansible.

Algunos de los roles están escritos dentro del mismo proyecto y otros son instalados desde **_galaxy.ansible_**, en el archivo **_requirements.yml_** se encuentran los roles que se instalarán.

## Uso

1. Instalar Ansible

```sh
sudo apt install ansible
```

2. Clonar el repositorio

```sh
git clone https://github.com/jeastman19/ansible-ubuntu-22.04
```

3. Instalar roles

```sh
ansible-galaxy install -r requirements.yml
```

4. Ejecutar playbook

```sh
./install.sh
```

# Anexos

## Roles externos

Existen en [Ansible Galaxy][ansible galaxy] una gran cantidad de roles que nos permiten automatizar la instalación de software y configuraciones, en este proyecto hemos utilizado los siguientes:

-   [Git](https://galaxy.ansible.com/geerlingguy/git)
-   [Oh my zsh](https://galaxy.ansible.com/gantsign/oh-my-zsh)
-   [Docker](https://galaxy.ansible.com/geerlingguy/docker)
-   [Kubectl](https://galaxy.ansible.com/andrewrothstein/kubectl)
-   [Docker Compose](https://galaxy.ansible.com/andrewrothstein/docker-compose)
-   [Minikube](https://galaxy.ansible.com/gantsign/minikube)

-   [Kubectl](https://galaxy.ansible.com/andrewrothstein/kubectl)

-   name: nvm
    src: stephdewit.nvm

-   name: oh-my-zsh
    src: gantsign.oh-my-zsh

-   name: vsc
    src: gantsign.visual-studio-code

-   name: terraform
    src: andrewrothstein.terraform

-   name: postman
    src: gantsign.postman

# TODO

-   Probar: [ansible-galaxy install jonaspammer.bootstrap](https://galaxy.ansible.com/jonaspammer/bootstrap)

[ansible galaxy]: https://galaxy.ansible.com/
