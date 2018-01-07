pipeline {
	agent any

	stages {
		stage('Build'){
			steps {
				build job: 'First-Maven-Project'
			}
		}

		stage('Deploy'){
			steps{
				build job: 'First-Deploy-Project'
			}
		}
	}
}
