# GBM-Ansible-Bitbucket
The repository contains the necessary files for automation of user addition to a Bitbucket repository. This saves time consuming task of manually adding users. A common use case would be to recollect the users that are going to be added to the Bitbucket repository through a survey/form and save it in a .csv/.txt format. Aftewards you can run the **main.yml** playbook through Ansible and the CLI, or the **tower_main.yml** playbook through Ansible Tower. 

# Pre-requisites
- **Ansible**: More info on installation [here](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).
- **Ansible Tower**: More info on installation [here](https://docs.ansible.com/ansible-tower/2.2.2/html/quickinstall/index.html).
- **Bitbucket repository**: More info on Bitbucket [here](https://bitbucket.org/product).
- Bitbucket user with administrative access/rights.

# Usage with Ansible CLI
Before launching, the playbook, edit the **vars.yml** file with your information as well as the file name which will retrieve the user's information.

# Usage with Ansible Tower
Before launching the playbook, add a survey to the job template to include the necessary variables and the users file to launch the template. 
