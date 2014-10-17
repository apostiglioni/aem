FROM ubuntu:14.04.1

RUN apt-get install -y software-properties-common \
	apt-add-repository ppa:ansible/ansible \
	apt-get update -y \
	apt-get install -y ansible

RUN ansible-playbook -i localhost author.yml --extra-vars "aem_quickstart_jar=aem-files/aem-6.0-quickstart.jar aem_license_file=aem-files/license.properties"

CMD start

EXPOSE 4502