pipeline {
    agent any
    
    tools {
        maven "maven" // the name you configured under "Global Tool Configuration"
    }
    stages {
        stage('clean') {
            steps {
                sh "mvn clean"
            }
        }
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        stage('Deploy') {
            steps {
                sh "mvn package"
            }
        }
    }
}