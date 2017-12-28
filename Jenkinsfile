pipeline{
	agent any

	stages{
		stage ('clone'){
		
			steps{
				git 'https://github.com/vatsalkumarr/MavenDemoRepo.git'
				}
		}
		
		
		stage ('compile'){
		
			steps{
				withMaven(maven : maven-3.3.9){
				 sh 'mvn clean install'
				}
			}
		
		}
		}
		}
	

