@Library('gcp-lab-jenkins-lib@main') _

pipeline {
  agent any

  stages {
    stage('Build, Push & Deploy FE App') {
      steps {
        pipelineWrapper(name: "fe-app-deploy") {
          buildPublishDeployApp(pipelineFile: "pipeline.yaml")
        }
      }
    }
  }
}
