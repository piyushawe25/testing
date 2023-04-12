pipeline {
  agent { 
		label 'blackduck' 
	}
  stages {
    stage('version') {
      steps {
        script{
                   dir("${env.WORKSPACE}") {
		bat 'python --version'
              }
             }
      }
    }
    stage('hello') {
      steps {
       script{
                   dir("${env.WORKSPACE}") {
		bat 'python test.py'
              }
             }
      }
    }
  }
}
