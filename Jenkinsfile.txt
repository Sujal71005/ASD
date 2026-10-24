
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Building the application...'
                bat 'echo Build completed successfully!'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running tests...'
                bat 'echo All tests passed!'
            }
        }

        stage('Finish') {
            steps {
                echo 'Jenkins CI practical completed!'
            }
        }
    }
}
