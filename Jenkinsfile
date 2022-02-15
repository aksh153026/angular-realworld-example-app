pipeline {
    
  agent {
      label 'master'
  }

  
    tools {
 
        nodejs 'NodeJS'
		maven 'MAVEN_HOME' 
        jdk 'jdk1.8' 
    }
    stages {
		stage('Checkout SCM') {
            steps {
def packageJSON = readJSON test: 'package.json'
def packageJSONVersion = packageJSON['version']
               
                echo packageJSONVersion
            }
        }
    }
}
