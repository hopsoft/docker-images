# Docker Images

The source used to build my public Docker images.

```bash
vagrant up
vagrant ssh
sudo docker build -t hopsoft/ruby-2.0 /vagrant/ruby-2.0
sudo docker push hopsoft/ruby-2.0
sudo docker build -t hopsoft/rbx-2.0 /vagrant/rbx-2.0
sudo docker push hopsoft/rbx-2.0
```
