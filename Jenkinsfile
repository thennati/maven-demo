pipeline {
  agent any
  stages {
    stage('maven') {
      steps {
        sh 'sh \'clean install package\''
        git(url: 'https://github.com/thennati/maven-demo', branch: 'master', poll: true, credentialsId: 'thennati')
      }
    }

  }
}