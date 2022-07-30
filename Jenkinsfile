pipeline {
    agent any
  stages {
    stage (smoke-google) {
      steps {
        script {
          #!/bin/bash
            
          . smoke.sh

          smoke_url_ok "http://google.com/"
              smoke_assert_body "search"
          smoke_report
        }
        sh "./smoke-google"
      }
    }
  }
}
