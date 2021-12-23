pipeline {
	agent {
		node {
			label 'nodejs'

		}
	}


	stages {
		stage (' Run Test') {
			steps {
				echo "running test....."
			}
			
		}
		stage ('deploy') {
			when { expression { env.GIT_BRANCH == 'origin/main'}}
			steps {
				echo "deploying......"
			}
		}
		}

		
	
}