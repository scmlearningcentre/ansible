# ansible example for Buildsetup
1. Setup Build Machine by installing JDK 1.8, Maven
  $ ansible-playbook buildsetup.yml 

2. Create EC2 machine & do not create dynamic inventory
  $ ansible-playbook createEc2.yml --skip-tags dynamicinventory

3. Create EC2 machine & add an entry to dynamic hosts file (by default)
  $ ansible-playbook createEc2.yml 

4. Create S3 bucket
  $ ansible-playbook createS3.yml

# ansible example for LAMP stack setup - Linux Apache Mysql PHP/Python
$ ansible-playbook lamp.yml
