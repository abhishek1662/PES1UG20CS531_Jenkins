pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS531-1 PES1UG20CS531.cpp'
                echo 'build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './PES1UG20CS531-1'
                echo 'test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'pipeline failed'
                }
            
   
    }
}
