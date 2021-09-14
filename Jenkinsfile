pipeline {
  agent {
    node {
      label 'CentOS7'
    }

  }
  stages {
    stage('Checkot') {
      steps {
        git(url: 'https://github.com/danny-ros/pipelines-dotnet-core.git', branch: 'master', changelog: true)
      }
    }

    stage('Build') {
      steps {
        sh 'sh dotnet build'
      }
    }

  }
}