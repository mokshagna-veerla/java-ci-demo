
pipeline {
    agent any

    tools {
        jdk 'JDK-25'
        maven 'Maven-3.10'
    }

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }

    post {
        success {
            echo 'Java project built successfully!'
        }
        failure {
            echo 'Java project build failed.'
        }
    }
}
