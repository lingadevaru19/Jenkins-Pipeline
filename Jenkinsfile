pipeline {
    agent any

    stages {
        stage('Build') {
          steps {
            echo 'Building the application...'
            // Add your build commands here, e.g., `mvn clean install` or `npm install`
          }
        }

        stage('Test') {
          parallel {
            stage('Unit Tests') {
              steps {
                echo 'Running unit tests...'
                // Commands for running unit tests, e.g., `mvn test` or `npm run test`
              }
            }

            stage('Integration Tests') {
              steps {
                echo 'Running integration tests...'
                // Commands for running integration tests
              }
            }
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deploying the application...'
            // Deployment commands, e.g., `kubectl apply` or `scp`
          }
        }
    }
}
