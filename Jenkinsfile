pipeline {
  agent {
    label 'master'
  }
  triggers {
    upstream(upstreamProjects: "jenkins-projectA/" + env.BRANCH_NAME.replaceAll("/", "%2F"), threshold: hudson.model.Result.SUCCESS)
  }
  stages {
    stage('Run echo vars') {
      steps {
        echo "Hello ${params.PERSON2}"
        echo "PASS_BRANCH_NAME: ${params.PASS_BRANCH_NAME}"
      }
    }
  }
}
  
