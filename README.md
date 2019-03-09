# Ansible role for Redis
Ansible role for Redis 5.0 for CentOS 7

## What's inside?
1. Redis 5.0 on port 6379, 3 databases by default

## Interesting dirs and files: 
```
/etc/redis.conf
/var/log/redis/redis.log
```

## Redis
#### Status
Verify if everything is ok:
```
redis-cli -h 127.0.0.1 ping
ss -an | grep 6379
``` 

#### Benchmark
Run the benchmark with 15 parallel connections, for a total of 10k requests, 
against local redis to test its performance.
```
redis-benchmark -h 127.0.0.1 -p 6379 -n 10000 -c 15
```
For more info execute: 
```
redis-benchmark --help
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
-[ ] test Redis with firewall

## License
Copyright (c) We Are Interactive under the MIT license.