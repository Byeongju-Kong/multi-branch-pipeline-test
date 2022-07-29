pipeline{
  agent any
  
  stages{
    stage('master ready') {
      steps{
        sh 'echo "ready"'
      }
    }

    stage('master test'){
      steps{
        sh 'echo "Test"'
      }
    }

    stage('master build'){
      steps{
        sh 'echo "Build"'
      }
    }

    stage('master deploy'){
      steps{
        sh 'echo "Deploy"'
      }
    }
  }
}
