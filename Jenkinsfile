pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "g++ PES2UG20CS335-1.cpp"
                echo "Build successfully."
            }
        }
        stage('Test') {
            steps {
                sh "a.exe"
              echo "Test successfully."
            }
        }
    }
    post {
        always {
            echo "Pipeline completed successfully."
        }
        failure {
            echo "Pipeline failed !!"
        }
    }
}
