#### build
 
```
➜  cmd_and_entrypoint git:(master) ✗ docker build -t test .
```

#### Run with default cmd
```
➜  cmd_and_entrypoint git:(master) ✗ docker run -it test
PING localhost (127.0.0.1) 56(84) bytes of data.
64 bytes from localhost (127.0.0.1): icmp_req=1 ttl=64 time=0.042 ms
64 bytes from localhost (127.0.0.1): icmp_req=2 ttl=64 time=0.083 ms
64 bytes from localhost (127.0.0.1): icmp_req=3 ttl=64 time=0.054 ms
```

#### Run with change cmd

```
➜  cmd_and_entrypoint git:(master) ✗ docker run -it test google.com
PING google.com (216.58.199.238) 56(84) bytes of data.
64 bytes from kix05s02-in-f238.1e100.net (216.58.199.238): icmp_req=1 ttl=37 time=25.1 ms
64 bytes from kix05s02-in-f238.1e100.net (216.58.199.238): icmp_req=2 ttl=37 time=24.3 ms
64 bytes from kix05s02-in-f238.1e100.net (216.58.199.238): icmp_req=3 ttl=37 time=22.1 ms
```