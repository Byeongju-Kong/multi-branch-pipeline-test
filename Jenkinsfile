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
  post {
      success {
          slackSend (channel: jenkins, color: '#00FF00', message: "SUCCESSFUL: Job '${env.JOB_NAME} [${env.BUILD_NUMBER}]' (${env.BUILD_URL})")
      }
      failure {
          slackSend (channel: jenkins, color: '#FF0000', message: "FAILED: Job '${env.JOB_NAME} [${env.BUILD_NUMBER}]' (${env.BUILD_URL})")
      }
  }

}
