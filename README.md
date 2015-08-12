# ansible-rancher

This ansible playbook provisions a set of Ubuntu 14.04 servers with a base Docker environment and [Rancher][r].

(only the master is installed automatically at the moment, since Rancher requires a token to set up slaves)

## Instructions

```
$ cp inventory.dist inventory.txt
$ vi inventory.txt
$ ansible-playbook --ask-pass --ask-sudo-pass -i inventory.txt main.yml
```

[r]: https://github.com/rancher/rancher