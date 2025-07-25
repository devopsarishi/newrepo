pipeline {
    agent any

    tools {
        maven 'Maven 3'   // Make sure this matches the name in Jenkins Global Tools Config
        jdk 'Java 17'     // Or Java 11 or any version you installed
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/devopsarishi/newrepo.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
