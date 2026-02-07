pipeline{
    agent any
    stages {
        stage ('Build') {
            steps {
                sh 'ls -l'

            }
        }
        stage ('test') {
            steps {
                sf 'whoami'

            }
        }
        stage ('deploy') {
            steps {
                sh 'top'

            }
        }
    }
}
