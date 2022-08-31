pipeline{
    agent { docker { image 'node:13.8' } }
    stages{
        stage('Build'){
            steps{
                echo "This is the build stage for maven"
                sh 'node --version'
            }
        }
        stage('Unit Tests'){
            steps{
                echo "This stage is for unit testing"
            }
        }
    }
    post{
        always{
            echo "The stages are completed"
        }
    }
}