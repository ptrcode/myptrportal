pipeline {
  agent none
  stages {
    stage('verify') {
      steps {
        echo 'verified resource'
      }
    }
    stage('Create VM') {
      steps {
        build(job: 'processjiraevents', quietPeriod: 1, propagate: true, wait: true)
      }
    }
  }
}