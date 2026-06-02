pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/Afreen7866/springboot-demo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Run') {
            steps {
                bat 'java -jar target/*.jar'
            }
        }
    }
}