# Ansible role for Redis
Ansible role for Redis 5.0 for CentOS 7

## What's inside?
1. Redis 5.0 on port 6379

## Interesting dirs and files: 
```
/etc/redis.conf
/var/log/redis/redis.log
```

## Tested on

## Installation
1. Navigate to Ansible's roles folder
2. Add the repo to git modules
    ```
    git submodule add https://github.com/budnerp/ansible_role_redis.git ansible_role_redis
    ```
3. Add the role to Ansible's playbook file
    ```    
    roles:
    [...]
        - ansible_role_redis
    [...]
    ```

## Other links
- Redis [https://redis.io/]()

## TO DO
-[ ] add dependencies

## License
Copyright (c) We Are Interactive under the MIT license.