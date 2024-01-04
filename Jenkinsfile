pipeline {
  agent any
  stages {
    stage('Execute') {
      steps {
        sh 'echo "Petando!!!"
        sh 'petepetepetepeteeee'
      }      
    }
    stage('Test') {
      steps {
          sh 'echo "Test!!!"
      }
    }
  }
  post {
    success {
       sh '''curl -X POST -H \'Content-Type: application/json\' -d \'{"chat_id": "902285901", "text": "YEEEEEEAAA!!!", "disable_notification": false}\'  https://api.telegram.org/bot6972167273:AAFfUCU_9JQyRVkQSbftk_Sc3FVqSpE_SEg/sendMessage
    }
    failure {
       sh '''curl -X POST -H \'Content-Type: application/json\' -d \'{"chat_id": "902285901", "text": "Ha petado :( ", "disable_notification": false}\'  https://api.telegram.org/bot6972167273:AAFfUCU_9JQyRVkQSbftk_Sc3FVqSpE_SEg/sendMessage

    }
  }
}
