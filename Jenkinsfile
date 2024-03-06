pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ working.cpp -o temp'
                 build job: 'PES1UG22CS806-1', wait: false
                 echo 'Build by CS806 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat working.cpp'
                echo 'Test by CS806 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS806 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
