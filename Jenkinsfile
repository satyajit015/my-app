pipeline {
    agent any

    stages {
        stage('Clean') {
            steps {
                echo 'Hello Repo'                              
                bat "mvn clean"
            }
        }
         stage('Build') {
            steps {
                bat "mvn compile"
            }
        }
        
        stage('Test') {
            steps {
                bat "mvn test"
            }
        }
        
        stage('Deploye') {
            steps {
                echo 'Hello Deploye'
                bat "mvn package"
            }
        }
    }
}

