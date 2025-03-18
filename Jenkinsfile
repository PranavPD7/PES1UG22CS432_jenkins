pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES1UG22CS432-1 newworking.cpp' // Compile hello.cpp
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES1UG22CS432-1'  // Run the compiled program
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying the application...'
                    // Deployment commands go here (if needed)
                }
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
