pipeline {

    agent any
    tools {
        maven 'maven-3.5.0'
        jdk 'JDK8' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn -f ./1.HelloWorld/HelloWorld-SB/pom.xml compile" 
        }
    }

         stage('Testing stage') {
             steps {
                bat "mvn -f ./1.HelloWorld/HelloWorld-SB/pom.xml test"
        }
    }

          stage('Deployment stage') {
              steps {
                bat "mvn -f ./1.HelloWorld/HelloWorld-SB/pom.xml deploy"
        }
    }

  }

}