pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "g++ -o PES2UG20CS335-1 PES2UG20CS335-1.cpp"
                echo "Build- successfully."
            }
        }
        stage('Test') {
            steps {
                sh "./PES2UG20CS335-1"
                echo "Test- successfully."
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy- successfully.'
            }
        }
    }
    post {
        always {
            echo "Pipe-line completed successfully."
        }
        failure {
            echo "Pipe-line failed !!"
        }
    }
}
