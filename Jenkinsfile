pipeline {
	agent any
	
	stages {
		stage('Emptying Workspace') {
			steps{
				cleanWs()
			}
		}		
		stage('build') {
			steps {
				sh 'ls'
				sh 'bash add_3_no.sh'
			}
		}
	}
	post {
		success {
			echo "Build Success !!"
		}
		failure {
			echo "Build failed !!"
		}
	}
}

