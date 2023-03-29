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
            sh '''#!/usr/bin/env bash

sudo apt update -y '''
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
  triggers {
    cron('*/10 * * * *')
  }
}