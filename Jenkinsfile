pipeline {
  agent {
    label 'master'
  }
  stages {
    stage {
      steps {
        echo "Hello ${params.PERSON2}"
        echo "PASS_BRANCH_NAME: ${params.PASS_BRANCH_NAME}"
      }
    }
  }
}
  
