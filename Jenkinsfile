// Declarative //
pipeline { 
	agent any
	
		stages{
		
			stage('Build') {
				steps {
					echo 'Building..'
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
