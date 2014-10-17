Windows users only:
- Install vagrant
- Install vagrant plugin install vagrant-hostsupdater
  This may require installation of:
    - Ruby
    - Ruby DevKit
    - gem install json -v '1.8.1'

- vagrant up
- vagrant ssh

- Linux users only:
- run init-host.sh --> installs ansible

- Install CQ:
ansible-playbook -i development site.yml --extra-vars "aem_quickstart_jar=aem-files/aem-6.0-quickstart.jar aem_license_file=aem-files/license.properties"


ansible-playbook -i development author.yml --extra-vars "aem_quickstart_jar=aem-files/aem-6.0-quickstart.jar aem_license_file=aem-files/license.properties"
