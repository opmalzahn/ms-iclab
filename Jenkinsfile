pipeline {
    agent any 
  

    stages {
        stage('Build') {
            steps {
                slackSend channel: '#builds-jenkins', color: 'good', message: 'Start job'
                echo 'TODO: build'
                bat 'mvnw clean compile -e'
            }
        }
        stage('Test') {
            steps {
                echo 'TODO: test'
                bat 'mvnw clean test -e'
            }
        }
        stage('Package') {
            steps {
                echo 'TODO: package'
                bat 'mvnw clean package -e'           
            }
        }
        stage('Run') {
            steps {
                echo 'TODO: run'
                bat 'mvnw spring-boot:run'                      
            }           
        }
        stage('Clean Workspace') {
            steps {     
                cleanWs()
<<<<<<< HEAD
=======
                slackSend channel: '#builds-jenkins', color: 'good', message: 'Finish job'
        }
}
