pipeline {
   
   agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build application'
            }
        }

        stage('Test') {
            steps {
                echo 'Test app'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy app'
            }
        }
    }
    
    post
	{
	
	always
		{
			emailext body: 'Testing Jenkins CICD', subject: 'Pipeline Status', to: 'shetesrushti11@gmail.com'
		}
	}
	
}
