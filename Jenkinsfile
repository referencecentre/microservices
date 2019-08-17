pipeline {

    agent any
    tools {
        maven 'maven-3.5.0'
        jdk 'JDK8' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn -f 1.HelloWorld/HelloWorld-SB/pom.xml clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn 1.HelloWorld/HelloWorld-SB/pom.xml test"
        }
    }

          stage('deployment stage') {
              steps {
                bat "mvn 1.HelloWorld/HelloWorld-SB/pom.xml deploy"
        }
    }

  }

}