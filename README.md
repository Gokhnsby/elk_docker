#sudo apt update

#sudo apt install apt-transport-https ca-certificates curl software-properties-common

#curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

#sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

#sudo apt update

#apt-cache policy docker-ce

#sudo apt install docker-ce

Then you need to edit /etc/sysctl.conf and add;
vm.max_map_count = 262144

#sudo systemctl status docker

#sudo docker pull sebp/elk:latest

#docker image ls  --installed

#sudo docker run -p 5601:5601 -p 9200:9200 -p 5044:5044 -it --name elk sebp/elk:latest

--if there is error about vm.max------------------------

vm.max_map_count = 262144 --increase that parameter to--
vm.max_map_count = 299000

#sysctl -w vm.max_map_count=299000

