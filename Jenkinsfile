pipeline {
    agent any
  stages {
    stage (test) {
        script {
            #!/bin/bash
            . smoke-google
        }
         steps {
            sh "bash ./smoke-google"
      }
    }
  }
}
