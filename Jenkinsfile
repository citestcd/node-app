pipeline {
  agent any


  stages {

    stage ('SCM checkout'){
            git "https://github.com/hiraxwahid/pytest/"
            }

    stage('Build') {
      steps {
        sh 'npm install'
         sh 'npm start'
      }
    }

    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}