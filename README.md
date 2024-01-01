HAZESOFT-T2
-----------
This repository contains an Ansible playbook to deploy a simple web application on a virtual machine.

Prerequisites
-------------
```
- Virtualization platform installed (e.g., VirtualBox, KVM)
- Ansible installed on your local machine
- HAZESOFT-T1 Repository link, including Docker-compose file
```

Usage
------
1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/HAZESOFT-T2.git
   ```
2. Get inside the repository:
```bash
    cd HAZESOFT-T2
```
3. Run the Ansible playbook:
```bash
  ansible-playbook -vi 192.168.1.95, -u abis --ask-become-pass deploy_task.yaml
   ```
Exmaple:
  ansible-playbook -i 'vm_IP', -u 'userName' --ask-become-pass deploy_task.yaml   

4. SSH into your virtual machine:
```bash
ssh your_vm_user@your_vm_ip
```
5. Run the following command on the virtual machine:
```bash
curl http://localhost:9000/site/index.html
```
You should see the message "You did it, Congratulations!!"
----------------------------------------------------------

