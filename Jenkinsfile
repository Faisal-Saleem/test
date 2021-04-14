pipeline {
  agent any
  stages {
    stage("Clean workspace") {
      steps {
        echo 'Cleaning workspace'
        cleanWs()
      }
    }
    stage("Git Checkout") {
      steps{
        git branch 'deploy'
      }
    }
    stage("Restore Packages") {
      steps {
        bat 'dotnet restore "${workspace}"'
        echo ${workspace}
      }
    }
  }
}
