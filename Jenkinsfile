pipeline {
  agent { 
		label 'blackduck' 
	}
  environment {

    PATH = "C:\\WINDOWS\\SYSTEM32"

}
	tools {
		python 'python-3.11.3'
	}
  stages {
    stage('version') {
      steps {
        script{
                   dir("${env.WORKSPACE}") {
		bat "python3 --version"
              }
             }
      }
    }
    stage('hello') {
      steps {
       script{
                   dir("${env.WORKSPACE}") {
		bat "python3 test.py"
              }
             }
      }
    }
  }
}
