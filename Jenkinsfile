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
packageJSON = readJSON file: 'package.json'
packageJSONVersion = packageJSON.version
               
                echo packageJSONVersion
            }
        }
    }
}
