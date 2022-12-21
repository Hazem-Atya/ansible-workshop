
## What is ansible?
Ansible is a suite of software tools that enables infrastructure as code.
Ansible works against multiple managed nodes or “hosts” in your infrastructure at the same time, using a list or group of lists known as inventory.

## How does it work?

By default, asnbile looks for the inventory file in /etc/ansible/hosts . To customize this, we create a conf file containing the directory of the inventory.

 ![image](https://user-images.githubusercontent.com/53778545/208709814-610349a6-1f16-4f7a-bf11-b70c1e1d24a0.png)

Inventory

![image](https://user-images.githubusercontent.com/53778545/208709840-2d297456-3718-4ddc-a3ca-9fddad0541ec.png)


Verify that the host is reachable via ssh (u may need to do chmod o -w . )

`ansible -m ping all`     
(this is not our useful ping, the useful ping doesn’t have w port but this command checks ssh connection)

![image](https://user-images.githubusercontent.com/53778545/208709986-a14e1c05-80b5-4767-9bd9-fc5fd040eb5b.png)
 
We need to add the key  (Fi nafs il staaaar)


![image](https://user-images.githubusercontent.com/53778545/208710009-8922927d-3724-41a1-8c59-efacf9c7b608.png)
 

 ![image](https://user-images.githubusercontent.com/53778545/208710072-d2056b9d-0f1b-4ea5-8202-17822f3f0e2c.png)


•	Creating a playbook.yaml

 ![image](https://user-images.githubusercontent.com/53778545/208710089-8cf63512-f72d-47a5-b3a4-6aac394e17a8.png)

Playbook => task => command 

`ansible-playbook playbook.yaml`     

![Untitled Diagram](https://user-images.githubusercontent.com/53778545/208862826-f5693a57-d9cb-4121-884e-860d63298778.jpg)
 
