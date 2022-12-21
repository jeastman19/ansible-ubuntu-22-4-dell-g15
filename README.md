
<table>
    <tr>
        <td>
            <img src="images/ansible-logo.png" width="200px">
        </td>
        <td>
            <img src="images/ubuntu-logo14.png" width="200px">
        </td>
    </tr>
</table>

# Ansible Dell G15 5515 con Ubuntu 22.04

Aprovicionamiento de la Laptop de trabajo

## Instalar Ansible

~~~sh
sudo apt install ansible
~~~

## Roles externos

Existen en [Ansible Galaxy][ansible galaxy] una gran cantidad de roles que nos permiten automatizar la instalación de software y configuraciones, en este proyecto hemos utilizado los siguientes:

* [Git](https://galaxy.ansible.com/geerlingguy/git)
* [Oh my zsh](https://galaxy.ansible.com/gantsign/oh-my-zsh)

[ansible galaxy]:https://galaxy.ansible.com/
