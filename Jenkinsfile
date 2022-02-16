pipeline {
    
  agent {
      label 'master'
  }


   
  
    tools {
  git 'Default'
        nodejs 'NodeJS'
		maven 'MAVEN_HOME' 
        jdk 'jdk1.8' 
    }
  
    stages {
		stage('Checkout SCM') {
      steps{
        script{
           [Monday 6:07 PM] sreekanth.t
def packageJSON = readJSON file: 'package.json'
def packageJSONVersion = packageJSON.version
          build_version = "${env.packageJSONVersion}.${env.BRANCH_NAME}.${BUILD_DATE}.${BUILD_TIMESTAMP}.${BUILD_ID}"
echo build_version

        }
      }
    }
}
}
