pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('stage') {
      steps {
        build(job: 'test', propagate: true, wait: true)
      }
    }
  }
  environment {
    stage = 'stage'
  }
}