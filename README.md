Helpers to:
- Setup NFS
- Setup /etc/hosts file

Edit the 'hosts' file and change the remote_user in the playbook.
Then run it as:
ansible-playbook -i hosts nfs.yml   --key-file=/home/johan/.ssh/id_rsa
and to setup the /etc/hosts file:
ansible-playbook -i hosts etchosts.yml   --key-file=/home/johan/.ssh/id_rsa