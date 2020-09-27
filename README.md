# Github---Jenkins---Docker


JENKINS INSTALLATION

curl --silent --location https://pkg.jenkins.io/redhat-stable/jenkins.repo | sudo tee /etc/yum.repos.d/jenkins.repo
rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
yum install java-1.8.0-openjdk-devel jenkins -y
systemctl daemon-reload;systemctl start jenkins;systemctl enable jenkins


DOCKER INSTALLATION

yum install -y yum-utils; yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo;yum install docker-ce docker-ce-cli containerd.io -y

systemctl start docker;systemctl enable docker;systemctl status docker