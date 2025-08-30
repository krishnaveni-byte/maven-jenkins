pipeline {
    agent any
    stages {
        stage('Example') {
           steps { bat "Hello testing pipeline" }
        }
    }
    post { 
	failure {
	   mail body: 'Hi krishna this is from uat branch', subject: 'The Pipeline failed', to: 'krisraj920@gmail.com'
        }
    }
}

