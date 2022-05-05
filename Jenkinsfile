pipeline {
  agent any
  stages {
    stage('dev_stage') {
      steps {
        echo 'hello'
      }
    }

    stage('qa_stage') {
      parallel {
        stage('qa_stage') {
          steps {
            echo 'hi QA'
          }
        }

        stage('qa_stage2') {
          steps {
            sleep 10
          }
        }

      }
    }

  }
  environment {
    ajil = 'ajil'
  }
}