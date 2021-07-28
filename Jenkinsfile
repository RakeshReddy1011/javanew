pipeline {
	agent any  
	stages {
		stage('Build') {
            steps {
                 sh 'mvn clean install'	    
                 echo 'buildis done'                  
            }                                         
		}
		
		
		stage('Test') {
		    steps {
			
			      echo 'testing the application'
			}
        }


        stage('Deploy') {
		    steps {
			      sh './deployment.sh'
			      echo 'Deploying the application'
			}
        }
	}
}
