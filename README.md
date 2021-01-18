# Integration of ansible, docker to launch a webserver

<img style="height: 60%;width: 40%;" src="https://github.com/akhilvmjr64/Webserver_ansible/blob/master/apache_docker_ansible.png">

By using the above playbook and files the [content](https://github.com/akhilvmjr64/Webserver_ansible/tree/master/content) in the folder content will be copied to the docker container and webserver will be launched

`It will first install the docker if it is not installed then it will start docker service then it will start the docker docker container`

## Operating system requirements
- It will work on `RedHat-8` operating system(not tested on other operating systems) with ansible installed in it(to install ansible use `pip3 install ansible`)

## Instructions:
- Use the file hosts in which you need to give the IP address/hostname of the node on which you want to launch a webserver you can even enter multiple hosts
- Use contents directory to change the content on the webpage
- Webserver will be hosted on one of the ports between 8000-8100 on the docker host

## Instructions while running the playbook:
- Fistly download the repository and then change your present working directory to the directory which you downloaded
- Then use the command `ansible-playbook docker.yml` to launch a webserver on docker container
