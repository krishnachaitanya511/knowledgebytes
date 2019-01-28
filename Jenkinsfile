pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh './gradlew check'
            }
        }
    }
    post {
        always {
            junit '/home/rchimaku/test-reports/*.xml'
        }
    }
}
