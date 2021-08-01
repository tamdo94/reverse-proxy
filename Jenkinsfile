pipeline {
    agent any

    tools { 
        maven 'Maven 3.6.3' 
        jdk 'JDK8' 
    }

    stages {
        stage('Build') {
            steps {
                sh '''
                    echo 'Building..'
                    cd app1
                    mvn clean install
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}