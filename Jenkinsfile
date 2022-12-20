pipeline {
   agent any
   tools{
       maven 'Maven'
       }

   stages {
	stage('Checkout') {
        steps {
		git 'https://github.com/Niravbhatt2006/maven-sample.git'
               }
            }
      stage('Build my job') {
        steps {
            sh 'mvn clean compile'
               }
            }
      stage('Package you App') {
         steps{
             sh 'mvn clean package'
               }
            }
//      stage('Sonar Checks') {
//	 steps{
//	    withSonarQubeEnv(installationName: 'Sonarscanner', credentialsId: 'SonarCloud') {
//  	    sh 'mvn clean package sonar:sonar'
 //    		}
  //	 }
      } 
   }         
}
