* Update OS packages
'''
sudo yum update -y
'''
* Install Docker
'''
sudo amazon-linux-extras install docker
'''
* Start Docker
'''
sudo service docker start
''''
*Enable it
'''
sudo systemctl enable docker
'''
*Add user to docker group
```
sudo usermod -a -G docker ec2-user
```