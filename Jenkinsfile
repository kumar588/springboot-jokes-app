pipeline {

  agent any
tools { 
        maven 'maven' 
        jdk 'jdk8' 
    }
  stages {
	stage('Build') { 
		    steps {
			   
            sh "mvn --version"
            sh "mvn clean install"
       
		    }
		}
     stage("Test"){
      steps{
        echo "Runing test cases"
        }
    }
    stage("Deploy"){
      steps{
        echo "Deploying application"
      }
    }
  }

}
