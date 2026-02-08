pipeline {
    agent any

    stages {
        stage('git clone') {
            steps {
                git branch: 'main', url: 'https://github.com/jagadeeshballajb/jenkins.git'
            }
        }
        stage ('Doker build') {
            steps {
              sh 'docker build -t dockerimage .'
            }
        }
        stage ('docker container') {
            steps {
                sh 'docker run -itd --name first0982 -p 1134:80 dockerimage'
            }
        }
    }
}
