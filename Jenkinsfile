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
        echo 'Workspace address ${workspace}'
      }
    }
  }
}
