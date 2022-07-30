pipeline {
    agent any
  stages {
    stage (test) {
        script {
            . smoke-google
        }
         steps {
            sh "bash ./smoke-google"
      }
    }
  }
}
