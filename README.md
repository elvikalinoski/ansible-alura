# Ansible Alura
Curso de Ansible na Alura

** Usando o debug e Executando o shell dentro da máquina **
 ```ansible -vvvv wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'```

**Executando o shell dentro da máquina**
 ```ansible wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'```