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
           def packageJSON = readJSON file: "package.json"
          bat "npm run build:single-spa:Lam"
        }
      }
    }
}
}
