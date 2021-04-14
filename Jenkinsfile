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
        bat 'dotnet build C:\\Users\\faisal.s\\source\\repos\\WebApplication1\\WebApplication1.sln'
      }
    }
  }
}
