pipeline {
    agent { docker { 
        image 'python:latest'
    } }
    environment {
        PROJECT_NAME="Jenkins Lessons"
        OWNER_NAME="Elena Borovik"
    }
    stages {
        stage('1-Build') {
            steps {
                echo 'Start Build'
                echo 'Building......'
                echo 'End Build'
            }
        }
        stage('2-Test') {
            steps {
                echo 'Start Test'
                echo "Project name is ${PROJECT_NAME}"
                sh "ls -la"
                echo 'End Test'
            }
        }
        stage('3-Deploy') {
            steps {
                echo 'Start Deploy'
                echo 'Deploying......'
                sh '''
                  echo "line 1"
                  echo "line 2"
                '''
                sh 'python --version'
                echo 'End Deploy'
            }
        }
    }
}
