# Docker Images

The source used to build my public Docker images.

## Build an Image

```bash
vagrant up
vagrant ssh
sudo docker build -t hopsoft/mri-2.0 /vagrant/mri-2.0
```

## Run an Image

```shell
vagrant up
vagrant ssh
sudo docker run -i -t hopsoft/rbx-2.0 bash
ruby -v
```

If you receive the error:

```
Error starting container 3e4798cd37ce: fork/exec /usr/bin/lxc-start: operation not permitted
```

Simply run again & things should work the 2nd time.

```
sudo docker run -i -t hopsoft/rbx-2.0 bash
```

This is a known Docker issue & should be [fixed soon](https://github.com/dotcloud/docker/pull/1489).

