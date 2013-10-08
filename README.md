# Docker Images

The source used to build my public Docker images.

## Build an Image

```bash
vagrant up
vagrant ssh
sudo docker build -t hopsoft/ruby-2.0 /vagrant/ruby-2.0
sudo docker push hopsoft/ruby-2.0
```

## Run an Image

_NOTE: The image in question must have been pushed to the [Docker index](https://index.docker.io/u/hopsoft/)._

```bash
vagrant up
vagrant ssh
sudo docker run -i -t hopsoft/rbx-2.0 bash
```
