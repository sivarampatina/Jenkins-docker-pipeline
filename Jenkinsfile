pipeline{
    agent 'any'
    environment{
        dockerHome = tool 'myDocker'
        mavenHome = tool 'myMaven'
        PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
    }
    stages{
        stage('Build'){
            steps{
                echo "This is the build stage for maven"
                sh 'node --version'
		sh 'docker version'
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