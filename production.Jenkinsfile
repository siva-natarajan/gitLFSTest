pipeline {
  agent any
  options {
    skipDefaultCheckout true
  }`
  stages {
    stage('clean_workspace_and_checkout_source') {
      steps {
        deleteDir()
        checkout scm
      }
    }
    stage('check git file size') {
        steps {
            sh("du -sh .git")
        }
    }
    stage('build') {
      steps {
        echo 'i build therefore i am'
      }
    }
  }
}
