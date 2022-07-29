pipeline{
  agent any
  
  tools {
      gradle 'gradle'
  }
  
  stages{
    stage('master ready') {
      sh 'echo "ready"'
    }

    stage('master test'){
      sh 'echo "Test"'
    }

    stage('master build'){
      sh 'echo "Build"'
    }

    stage('master deploy'){
      sh 'echo "Deploy"'
    }
  }
}
