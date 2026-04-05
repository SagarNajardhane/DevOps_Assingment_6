pipeline {

    agent any

    tools {
        maven 'Maven3'
        jdk 'Java17'
    }
    

    triggers {
        
        githubPush()
    }

    stages {

        stage('Build') {
            steps {
                bat 'mvn -v'
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }

    }

}
