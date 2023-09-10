pipeline {
  agent any {
    stages {
      stage ('check out') {
        steps {
          checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Sdupaku1/ci-cd-demo-java.git']])
        }
     stage ('build and test') {
        sh 'mvn test'
     }
      }
    }
  }
}
