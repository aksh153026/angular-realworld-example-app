pipeline {
    
  agent {
      label 'master'
  }
def packageJSON = readJSON file: 'package.json'

                echo packageJSON['version']
  
    tools {
 
        nodejs 'NodeJS'
		maven 'MAVEN_HOME' 
        jdk 'jdk1.8' 
    }
    stages {
		stage('Checkout SCM') {
            steps {
echo packageJSON['version']
            }
        }
    }
}
