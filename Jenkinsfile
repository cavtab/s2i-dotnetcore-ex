pipeline {
  agent any
  stages {
    stage('Trigger OpenShift Build') {
      steps {
        openshiftBuild 'test-app-demo-jenkins'
      }
    }
    stage('Trigger OpenShift Deploy') {
      steps {
        openshiftDeploy 'test-app-demo-jenkins'
      }
    }
  }
}