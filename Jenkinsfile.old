pipeline {
    agent any

    stages {
        stage ('Build Image') {
            steps {
                script {
                    dockerapp = docker.build("chagasgb/todo-list:${env.BUILD_ID}", '-f ./src/Dockerfile ./src') 
                }                
            }
        }
    }
}