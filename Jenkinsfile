pipeline{
  agent{
    label 'master'
  }
  stages{
    stage('Build Jenkins Jobs'){
      steps{
        sh 'sudo jenkins-jobs --conf server.ini update .'
      }
    }
  }

  post {
    always {
      deleteDir()
    }
  }
}
