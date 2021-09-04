pipeline {
	// agent any
	agent {docker { image 'node:alpine3.11'} }
	stages {
		stage('Build') {
			steps {
					sh 'node --version'
					echo "Build"
			}
		}
		stage('Test') {
			steps {
					echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
					echo "Integration Test"
			}
		}	
	} 
	post {
		always {
			echo 'im awesome. I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when you fail'
		}
	}
}
