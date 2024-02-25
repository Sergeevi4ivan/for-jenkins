pipeline {
    agent any 
    stages {
        stage('Clone the repo') {
            steps {
                echo 'clone the repo'
                sh 'rm -fr html'
                sh 'git clone https://github.com/Sergeevi4ivan/for-jenkins.git'
            }
        }
        stage('push repo to remote host') {
            steps {
                echo 'connect to remote host and pull down the latest version'
                sh 'ssh -i ~/working.pem ec2-user@35.176.182.32 sudo git -C /var/www/html pull'
            }
        }
        
        }
    }
}
