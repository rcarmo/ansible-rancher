# ansible-rancher

This ansible playbook provisions an Ubuntu 14.04 server with a base Docker environment and [Rancher][r].

## Instructions

```
$ cp inventory.dist inventory.txt
$ vi inventory.txt
$ ansible-playbook --ask-pass --ask-sudo-pass -i inventory.txt main.yml
```

[r]: https://github.com/rancher/rancher