pipeline {
  agent any

  stages {
    stage('Clone Repo') {
      steps {
        git 'https://github.com/Yoganandha-S/mywebsite.git'
      }
    }

    stage('Build') {
      steps {
        echo 'No build needed for static site'
      }
    }

    stage('Deploy') {
      steps {
        sh '''
          sudo cp jenkins.html /var/www/html/jenkins.html
          echo "Deployment complete!"
        '''
      }
    }
  }
}
