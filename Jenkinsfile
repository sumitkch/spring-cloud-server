pipeline{
	agent  any
	stages{
		stage(“version”){
			withMaven (maven : ‘M3’){
				sh ‘mvn --version’
			}
			
		}
		stage(“clean”){
			withMaven (maven : ‘M3’){
				sh ‘mvn clean’
			}
			
		}
		stage(“test”){
			withMaven (maven : ‘M3’){
				sh ‘mvn test’
			}
			
		}
		stage(“build”){
			withMaven (maven : ‘M3’){
				sh ‘mvn install’
			}
			
		}
	}
}