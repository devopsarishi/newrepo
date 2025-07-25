pipeline {
    agent any

    tools {
        maven 'maven3'
        jdk 'java17'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

