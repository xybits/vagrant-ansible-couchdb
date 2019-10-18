
# vagrant-ansible-couchdb

Example of CouchDB replication with three servers.


## Prerequisites:

Download and install the following tools:

- [VirtualBox & Extension Pack](https://www.virtualbox.org/wiki/Downloads)
- [Vagrant](https://www.vagrantup.com/downloads.html)
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) 2.8+

## Running the code

- Status:
  ```bash
  -:$ vagrant status
  ```
- Instantiate servers:
   ```bash
   -:$ vagrant up --provision couchdb01 couchdb02 couchdb03
   ```
- Connect to a server
  - Point browser to: http://<couchdb0[1|2|3]>:5894/_utils/
  - Use admin username/password to login
  - Browse to: http://<couchdb0[1|2|3]>:5894/_membership

