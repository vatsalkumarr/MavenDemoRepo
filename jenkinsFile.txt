pipeline{
	agent any

	stages{
		stage ('clone'){
		
			steps{
				withMaven(maven : maven){
				git 'https://github.com/vatsalkumarr/MavenDemoRepo.git'
				 
				}
			}
		
		}
		stage ('compile'){
		
			steps{
				withMaven(maven : maven){
				 sh 'mvn clean install'
				}
			}
		
		}
	}
}
