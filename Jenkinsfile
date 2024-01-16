pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Add your build commands here
                echo 'Building...'
                // For example: sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Add your test commands here
                echo 'Testing...'
                // For example: sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Add your deployment commands here
                echo 'Deploying...'
                // For example: sh './deploy.sh'
            }
        }
    }

    post {
        always {
            // Steps to perform after the pipeline runs, regardless of the result
            echo 'Pipeline execution complete.'
        }
        success {
            // Steps to perform if the pipeline is successful
            echo 'Build succeeded.'
        }
        failure {
            // Steps to perform if the pipeline fails
            echo 'Build failed.'
        }
    }
}
