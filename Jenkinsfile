pipeline {
  agent { 
		label 'blackduck' 
	}
  stages {
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    stage('hello') {
      steps {
        sh 'python3 test.py'
      }
    }
  }
}
