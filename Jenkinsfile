pipeline {
	agent {
		node {
			label 'nodejs'

		}
	}

	stages {
		stage (' RUn Test') {
			parallel {
				stage ('Backend Tests') {
					steps {
						sh 'node ./backend/test.js'
					}
				}

				stage ('Front Test') {
					steps {
						sh 'node ./frontend/test.js'
					}
				}
			}
		}

		
	}
}