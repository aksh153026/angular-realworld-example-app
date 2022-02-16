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

def packageJSON = readJSON file: 'package.json'
def packageJSONVersion = packageJSON.version
         def build_version = "${env.packageJSONVersion}.${env.BRANCH_NAME}.${BUILD_ID}"
echo packageJSONVersion

        }
      }
    }
}
}
