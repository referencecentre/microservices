pipeline{
	agent any
	
	stages{
		stage('Compile Stage'){
			steps{
				maven(maven : 'Maven'){
					 mvn clean compile
				}
			  }
		   }
		stage('Testing Stage'){
			steps{
				maven(maven : 'Maven'){
					 mvn test
				}
			  }
		   }
		stage('Deployment Stage'){
			steps{
				maven(maven : 'Maven'){
					 mvn deploy
				}
			  }
		   }
	
	    }

}