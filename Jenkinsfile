pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'this is the build job'
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        echo 'this is the test job'
        sh 'npm test'
      }
    }

<<<<<<< HEAD
    stage('package') {
      steps {
        echo 'this is the package job'
        sh 'npm run package'
      }
=======
// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs'
>>>>>>> b30c4db597f3c23fffd95e7b6a2de5eeeda256fc
    }

<<<<<<< HEAD
    stage('artifact') {
      steps {
        archiveArtifacts '**/distribution/*.zip'
      }
=======
    stages{
        stage(‘Build’){
            steps{
                echo 'this is the first job - Build'
                sh ‘npm install'
            }
        }
        stage(’Test’){
            steps{
                echo 'this is the second job - Test'
                sh ‘npm test'
            }
        }
        stage(‘Package’){
            steps{
                echo 'this is the third job - Package'
                sh ‘npm run package'
            }
        }
>>>>>>> b30c4db597f3c23fffd95e7b6a2de5eeeda256fc
    }

  }
  tools {
    nodejs 'nodejs'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }

  }
}
