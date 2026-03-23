pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/SagarNajardhane/DevOps_Assingment_6.git'
            }
        }

        stage('Build') {
            steps {
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
