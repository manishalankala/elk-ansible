------------------------------------------------------------------------------------------------------------------------------------------------------------

create instance in azure ubuntu 18

### Docker
~~~

sudo apt update
sudo apt upgrade
sudo apt-get install curl apt-transport-https ca-certificates software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt update
sudo apt install docker-ce
~~~

### ansible

~~~
apt-get install python-pip python-dev
apt install python3-pip
sudo apt install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt update
sudo apt-get install ansible -y

~~~

### Specific version

~~~
sudo add-apt-repository --update ppa:ansible/ansible-2.9.7
sudo apt install ansible

or 

sudo apt-get install python-pip python-dev
sudo -H pip install ansible==2.9.7
~~~


### jenkins

~~~
sudo apt update	
sudo apt install openjdk-8-jdk -y
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update
sudo apt install jenkins -y
sudo systemctl start jenkins
sudo systemctl status jenkins

~~~


### Instance

![image](https://user-images.githubusercontent.com/33985509/127038871-eb1d3376-c800-439b-8659-aadc9424b365.png)

### Network

![image](https://user-images.githubusercontent.com/33985509/127039248-9ddfe93d-9192-4b1d-ad1c-9756e8463a29.png)


### jenkins
![image](https://user-images.githubusercontent.com/33985509/127039391-a190c8c7-9a0a-4117-8d99-5bb09c850469.png)

![image](https://user-images.githubusercontent.com/33985509/127039571-b127be02-4ad5-4bb0-a972-41266520150b.png)

![image](https://user-images.githubusercontent.com/33985509/127039815-736f0c62-09f8-4f93-9525-47dad20fd1a0.png)

![image](https://user-images.githubusercontent.com/33985509/127039862-a9783bfd-d120-4a6b-a2e4-a6e0f1922791.png)

![image](https://user-images.githubusercontent.com/33985509/127039928-46b905a5-3260-466c-aa84-7c4bda137ebe.png)

![image](https://user-images.githubusercontent.com/33985509/127040044-da29f350-1009-4e3c-9ac1-f1f3ce0a733a.png)


![image](https://user-images.githubusercontent.com/33985509/127040116-d6c4d1e8-4c71-4c0e-93b5-d2441c206f4a.png)

![image](https://user-images.githubusercontent.com/33985509/127040268-f7bcf572-ca9f-4898-bb91-ab87a01fff0b.png)

![image](https://user-images.githubusercontent.com/33985509/127040442-d72aa2ef-fcd4-41a8-96ad-d0adb20cbc16.png)
