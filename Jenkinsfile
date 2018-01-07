pipeline {
	agent any

	stages {
		stage('Build'){
			steps {
				build job: 'First-Maven-Project'
			}
			post {
				success {
					archiveArtifacts artifacts: '**/*.war'
				}
			}
		}

		stage('Deploy'){
			steps{
				build job: 'First-Deploy-Project'
			}
		}
	}
}
