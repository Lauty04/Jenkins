pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'cat /etc/etc/passwd'
            sh 'echo \'ejecutado con exito\''
          }
        }

        stage('step2') {
          steps {
            sh 'echo \'step2\''
          }
        }

      }
    }

    stage('stage2') {
      steps {
        sh 'sleep 15'
      }
    }

    stage('notificaciones') {
      steps {
        sh '''curl -X POST -H "Content-Type: application/json" -d "{\\"chat_id\\": \\"5419757145\\", \\"text\\": \\"Falló la tarea $JOB_NAME!! $BUILD_NUMBER,  \\", \\"disable_notification\\": false}" https://api.telegram.org/bot6421695221:AAFvC_xdV-RTxlAuH0_Fdahu0TMLXFHkWgU/sendMessage

'''
      }
    }

  }
}