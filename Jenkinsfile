pipeline {
  agent { 
		label 'blackduck' 
	}
  stages {
    stage('version') {
      steps {
        sh 'python --version'
      }
    }
    stage('hello') {
      steps {
        sh 'python test.py'
      }
    }
  }
}
