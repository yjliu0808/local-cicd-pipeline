pipeline {
  agent any

  triggers {
    pollSCM('H/3 * * * *')  // 每 3 分钟轮询
  }

  stages {
    stage('Pull Code') {
      steps {
        checkout scm
        echo '代码已拉取-1'
      }
    }
  }
}
