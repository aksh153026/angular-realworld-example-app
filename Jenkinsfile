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
  def packageJSON = readJSON file: 'package.json'
    stages {
		stage('Checkout SCM') {
            steps {
echo packageJSON['version']
            }
        }
    }
}
