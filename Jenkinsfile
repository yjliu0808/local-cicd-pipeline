pipeline {
  agent any

  triggers {
    pollSCM('H/3 * * * *')  // 每 3 分钟拉取 GitHub 仓库一次
  }

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Build') {
      steps {
        echo '构建中...'
        // sh 'npm install' 或 'mvn clean install'
      }
    }

    stage('Test') {
      steps {
        echo '测试中...'
      }
    }

    stage('Deploy') {
      steps {
        echo '部署中...'
      }
    }
  }
}
