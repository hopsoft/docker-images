## Ports that should be forwarded.

* nginx: 80
* carbon: 2003
* statsd: 8125


## Examples

Bash

```
mkdir /var/log/graphite
docker run -i -t -p 5000:80 -p 2003:2003 -p 8125:8125/udp -v /var/log/graphite:/var/log hopsoft/graphite-0.9 bash
/opt/hopsoft/graphite-0.9/start
```

Daemonized

```
mkdir /var/log/graphite
docker run -d -p 5000:80 -p 2003:2003 -p 8125:8125/udp -v /var/log/graphite:/var/log hopsoft/graphite-0.9 /opt/hopsoft/graphite-0.9/start
```

