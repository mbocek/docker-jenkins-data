Jenkin Data
============

Docker recipe for jenkins volume.

Run data image: 
```
sudo docker run --name jenkins-data mbocek/jenkins-data
```

Run jenkins image which use data image
```
sudo docker run -d  -m=1g --name jenkins -p 8080:8080 --volumes-from jenkins-data jenkins:latest
```
