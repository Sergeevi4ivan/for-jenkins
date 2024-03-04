pipeline {
    agent any 
    stages {
        stage('Clone the repo') {
            steps {
                echo 'clone the repo'
                sh 'rm -fr for-jenkins'
                sh 'git clone https://github.com/Sergeevi4ivan/for-jenkins.git'
            }
        }
        stage('push repo to remote host') {
            steps {
                echo 'connect to remote host and pull down the latest version'
                sh 'cat /home/ivan/Рабочий стол/folder/password.txt | sudo -S /opt/tomcat/webapps/forTestJenkins pull'
            }
    }
}
}
