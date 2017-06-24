pipeline {
agent any 
stages {
stage('build') {
steps {
sh 'docker build -t /tmp/centos:v1 Dockerfile'
sh 'docker image ls'
}
}
}
}
