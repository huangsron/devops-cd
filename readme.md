## install ansible 
sudo apt-get install ansible

## CD
### get install docker-compose role
ansible-galaxy install ypsman.docker_compose

### deploy container
ansible-playbook -i inventory playbooks/deploy.yml -e "build_version=dev applyHosts=nginx target=dev"