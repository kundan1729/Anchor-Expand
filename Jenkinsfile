pipeline {
  agent any

  stages {
    stage('Clone') {
      steps {
        git 'https://github.com/kundan1729/Anchor-Expand.git'
      }
    }

    stage('Build') {
      steps {
        echo 'No build needed for HTML files.'
      }
    }

    stage('Deploy') {
      steps {
        sh '''
          mkdir -p deploy
          cp index.html deploy/
          echo "Deployment complete. index.html moved to deploy folder."
        '''
      }
    }
  }
}
