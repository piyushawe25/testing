pipeline {
  agent { 
		label 'blackduck' 
	}
  stages {
    stage('version') {
      steps {
        script{
                   dir("${env.WORKSPACE}") {
		bat 'python3 --version'
              }
             }
      }
    }
    stage('hello') {
      steps {
       script{
                   dir("${env.WORKSPACE}") {
		bat 'python3 test.py'
              }
             }
      }
    }
  }
}
