### Docker Installation Steps in Amazon Linux
* For reference,
```
https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-container-image.html#create-container-image-install-docker
```
### Install Docker in AWS Linux 2
* Update OS packages
```
sudo yum update -y
```
* Install Docker
```
sudo amazon-linux-extras install docker
```
* Start Docker
```
sudo service docker start
```
* Enable it
```
sudo systemctl enable docker
```
* Add user to docker group
```
sudo usermod -a -G docker ec2-user
```