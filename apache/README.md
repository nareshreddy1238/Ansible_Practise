
How do we run roles

1. create playbook <demo.yml> 
---                                                               
- name: update os both ubuntu & centos server                       
  hosts: all                                                        
  become: yes                                                                                                                         
  roles:                                                              
  - /home/centos/apache                                         
 ...                         
 
 2. run the playbook
   > ansible-playbook -i aws.ini demo.yaml
