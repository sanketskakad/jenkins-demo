pipeline {
  agent any
  stages {
    stage('clonecode') {
      steps {
        git(url: 'https://github.com/sanketskakad/jenkins-demo', branch: 'main')
      }
    }

    stage('log') {
      steps {
        sh 'pwd'
        sh 'ls -a'
      }
    }

    stage('BuildJob') {
      steps {
        npm 'install'
        npm 'run build'
        sh 'ls -a'
        sh 'cd build'
        sh 'ls'
      }
    }

  }
}