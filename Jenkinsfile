pipeline {
  agent any
  stages {
    stage("Clean workspace") {
      steps {
        echo 'Cleaning workspace'
        cleanWs()
      }
    }
    stage("Checkout") {
      steps {
        echo 'Checkout Updated Code'
        git branch: 'master', url:'https://github.com/Faisal-Saleem/test'
      }
    }
    stage("Build App") {
      steps {
        echo 'Builing App...'
        bat 'dotnet build \\WebApplication1\\WebApplication1.sln'
      }
    }
  }
}
