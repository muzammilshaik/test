pipeline {
  agent any
  stages {
    stage('initial step') {
      steps {
        echo 'this is your first step'
      }
    }

    stage('second step') {
      steps {
        build(job: 'this is the first job', quietPeriod: 5, wait: true, propagate: true)
      }
    }

  }
}