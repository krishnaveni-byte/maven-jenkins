pipeline {
    agent any
    stages {
        stage('Example') {
           steps { bat "Hello testing pipeline" }
        }
    }
    post { 
	failure {
	   mail body: 'Hi krishna this is from master branch', subject: 'The Pipeline failed', to: 'krisraj920@gmail.com'
        }
    }
}

