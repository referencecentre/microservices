pipeline{
	agent any
	
	stages{
		stage('Compile Stage'){
			steps{
				withMaven(maven : 'maven-3.5.0'){
					 bat 'mvn clean compile'
					 echo 'compile'
				}
			  }
		   }
		stage('Testing Stage'){
			steps{
				withMaven(maven : 'maven-3.5.0'){
					 bat 'mvn test'
				}
			  }
		   }
		stage('Deployment Stage'){
			steps{
				withMaven(maven : 'maven-3.5.0'){
					 bat 'mvn deploy'
				}
			  }
		   }
	
	    }

}