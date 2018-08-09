pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            svn(changelog: true, poll: true, url: 'wq')
          }
        }
        stage('22') {
          steps {
            build(job: 'qwwe', wait: true, propagate: true, quietPeriod: 2)
          }
        }
      }
    }
  }
}