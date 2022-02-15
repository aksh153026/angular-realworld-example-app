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
            steps {
              def packageJSON = readJSON file: 'package.json'
              echo packageJSON['version']
            }
        }
    }
}
