1. The Ansible Playbook (install_apps.yml)
Save the following YAML code to a file named install_apps.yml on your server:

2. How to Run It
Method A: Run directly on your server
If you already SSH'd into your server, run these two commands:

Syntax Check (Optional):
~~~~
Bash
ansible-playbook install_apps.yml --syntax-check
~~~~
Execute the Playbook:
~~~
Bash
sudo ansible-playbook install_apps.yml
~~~
Apply Docker Permissions:
After running, refresh your group permissions so you can run Docker without sudo:
~~~~
Bash
newgrp docker
~~~~
