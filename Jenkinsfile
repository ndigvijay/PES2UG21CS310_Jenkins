  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o output main/main.cpp'
        echo 'Build Successful!'
      }
    }
    stage('Test') {
      steps {
        sh './output'
        echo 'Test Successful!'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Successfully deployed!'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline Failed!'
    }
  }
}