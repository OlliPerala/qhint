pipeline {
  agent any
  stages {
    stage('kehi') {
      agent any
      steps {
        build 'ollitest'
        archiveArtifacts(onlyIfSuccessful: true, artifacts: 'ollitest')
      }
    }
    stage('testi') {
      steps {
        build 'ollitest2'
      }
    }
    stage('tuotanto') {
      steps {
        build 'olli3'
      }
    }
  }
}