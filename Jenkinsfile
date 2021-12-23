pipeline {
	agent {
		node {
			label 'nodejs'

		}
	}
	environment {
		USER = 'root'
		PATH = "/root:$PATH"
	}


	stages {
		stage (' Run shell script') {
			steps {
				sh 'oci os bucket list'
			}
			
		}

		}

		
	
}