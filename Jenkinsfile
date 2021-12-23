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
				sh '/root/bin/oci os bucket list'
			}
			
		}

		}

		
	
}