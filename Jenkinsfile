pipeline {
  agent any
  stages {
    stage("Clean workspace") {
      steps {
        echo 'Cleaning workspace'
        cleanWs()
      }
    }
    stage("Build App") {
      steps {
        echo 'Builing App...'
        bat 'msbuild.exe ${workspace}\\WebApplication1\\WebApplication1.sln'
      }
    }
  }
}
