# Ansible Alura
Curso de Ansible na Alura

**Usando o debug e Executando o shell dentro da máquina**
 ```ansible -vvvv wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'```

**Executando o shell dentro da máquina**
 ```ansible wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'```

**Executa o playbook do ansible**
ansible-playbook provisioning.yml -u vagrant -i hosts

Passando variaveis na linha de comando
ansible-playbook -i hosts --extra-vars 'wp_db_name=wordpress_db' provisioning.yml