# Deploy Tarantool Cartridge application

First, start two vagrant virtual machines:

```bash
$ git clone https://github.com/tarantool/ansible-cartridge.git tarantool-cartridge
$ vagrant up
```

Then, deploy Tarantool Cartridge application on this machines and set up cluster topology:

```bash
$ ansible-playbook -i hosts.yml playbook.yml
```

Then, go to the http://localhost:8181/admin/cluster/dashboard and enjoy!
