pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        echo '🔄 Checking out source code...'
        checkout scm
      }
    }

    stage('Install Dependencies') {
      steps {
        echo '📦 Installing npm packages...'
        sh 'npm install'
      }
    }

    stage('Run App') {
      steps {
        echo '🚀 Running Node.js application...'
        sh 'node index.js'
      }
    }
  }
}

