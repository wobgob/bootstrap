# Bootstrap
Scripts to bootstrap the Wobblin' Goblin servers.

## Requirements
* Bash
* Ansible
* [MySQL collection for Ansible](https://github.com/ansible-collections/community.mysql)

## Usage
1. Create a `.env` file like the following

```
DISCORD_BOT_TOKEN=NzYwMTI1MDA2NDI4MjQxOTUy.X3Hfkw.EjIL6vI9XPHvhp9mmh6XZf7RoMo
MYSQL_USER=wobgob
MYSQL_PASSWORD=wobgob
MYSQL_HOST=127.0.0.1
MYSQL_PORT=3306
```

2. Create an `inventory.ini` file like the following

```
[apps]
winter.wobgob.org ansible_host=157.163.142.201

[db]
ruby.wobgob.org ansible_host=106.68.33.222
```

3. Run the playbook

```
$ ./play site.yml
```
