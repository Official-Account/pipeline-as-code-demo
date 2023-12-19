// Declarative //
pipeline { 
	agent any
	
		stages{
		
			stage('Build') {
				steps {
					echo 'Building..'
					sh 'echo "SSH private key is located at $SSH_CREDS"'
				}
			}
			stage('compile'){
				steps{
					sh "javac Hello.java"
				}
			}
			stage('run'){
				steps{
					sh "java Hello"
				}
			}
		}
}
