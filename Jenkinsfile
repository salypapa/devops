pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building.'
          }
        }

        stage('build2') {
          steps {
            sh 'echo "build2"'
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'Testing.'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying.'
      }
    }

  }

}
