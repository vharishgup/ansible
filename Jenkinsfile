pipeline {
agent any 
stages {
stage('build') {
steps {
sh 'yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo'
sh 'yum clean all'
sh 'yum install -y docker-ce-17.03.0.ce-1.el7.centos'
sh 'systemctl docker start'
sh 'docker build -t /tmp/centos:v1 Dockerfile'
sh 'docker image ls'
}
}
}
}
