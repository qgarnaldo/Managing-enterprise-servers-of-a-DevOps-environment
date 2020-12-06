###How to create an Ansible Configuration
1. Make sure that your system has the updated version of ansible, you can check by using the command `ansible --version`
2. To check if it's correctly installed, check the puthon version and check if it would reflect python 3. If it is python 3, then you're good to go.
3. Create ansible.cfg file on your desired directory where you will be accessing the ansible.
4. Populate the "ansible.cfg" with basic information needed like the path of the inventory, default remote user, and host verification.
###How to create an Ansible Inventory
1. Creae a file name inventory.
2. Use the vim command to input the IP address of the desired server to match with. (On other cases that I've experienced if there are more than one OS to be used, you can also indicate at the side of the IP address the username of the server by using `ansible_user=<username>`
###How to create an Ad-hoc Ansible command with setup and shell module
1. Make sure that ansible.cfg and inventory is setup.
2. Use the command `ansible all -m ping` to verify hosts. (In the case it won't push through, try using ssh username@ip first. If it persists, check the network on the VM settings)
3. Use the command `ansible all -m shell -a`
4. Verify using ls command.
