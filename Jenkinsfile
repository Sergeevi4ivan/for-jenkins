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
                sh 'git pull /opt/tomcat/webapps/forTestJenkins'
            }
    }
}
}
