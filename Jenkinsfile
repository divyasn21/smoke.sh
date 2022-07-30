pipeline {
    agent any
  stages {
    stage (smoke-google) {
      steps {
        script {
          . smoke.sh

          smoke_url_ok "http://google.com/"
              smoke_assert_body "search"
          smoke_report
        }
        sh "bash ./smoke-google"
      }
    }
  }
}
