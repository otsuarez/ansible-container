# ansible-container

Dockerfile for running ansible-playbook inside a container


```
docker login --username=otsuarez
docker build -f Dockerfile -t otsuarez/ansible .
docker run --name ansible-playbook --rm   otsuarez/ansible --version
docker push otsuarez/ansible
```


```sh
$ docker run --name ansible-playbook --rm   otsuarez/ansible --version
ansible-playbook 2.8.5
  config file = None
  configured module search path = ['/root/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /ansible/lib/ansible
  executable location = /ansible/bin/ansible-playbook
  python version = 3.7.4 (default, Aug 21 2019, 00:19:59) [GCC 8.3.0]
```

