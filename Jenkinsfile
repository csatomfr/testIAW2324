pipeline {
  agent any
  stages {
    stage('Telegram') {
      steps {
        telegramSend(chatId: 902285901, message: 'sasdsa')
        sh '''curl -X POST -H \'Content-Type: application/json\' -d \'{"chat_id": "902285901", "text": "YEEEEEEAAA!!!", "disable_notification": false}\'  https://api.telegram.org/bot6972167273:AAFfUCU_9JQyRVkQSbftk_Sc3FVqSpE_SEg/sendMessage

'''
      }
    }

  }
}