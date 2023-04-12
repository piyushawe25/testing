pipeline {
  agent { 
		label 'blackduck' 
	}
  stages {
    stage('version') {
      steps {
        script{
                   dir("${env.WORKSPACE}") {
		bat 'test.bat'
              }
             }
      }
    }
    stage('hello') {
      steps {
       script{
                   dir("${env.WORKSPACE}") {
		bat 'test.bat'
              }
             }
      }
    }
  }
}
