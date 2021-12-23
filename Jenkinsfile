pipeline {
	agent {
		node {
			label 'nodejs'

		}
	}
	parameters {
		booleanParam (name: "RUN_FRONT_END_TEST", default: true)
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

					when { expression { param.RUN_FRONT_END_TEST}}
					steps {
						sh 'node ./frontend/test.js'
					}
				}
			}
		}

		
	}
}