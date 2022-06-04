import java.text.SimpleDateFormat

pipeline {
    agent {
        label "demoAgent"
    } 
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps steps {
                 // java 라이브러리를 이용하여 날짜를 구한다 
                 script {
                    def dateFormat = new SimpleDateFormat("yyyyMMdd")
                    def date = new Date()
                
                    today = dateFormat.format(date)
                    echo today
                    
                }                
            } 
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        always{
            echo 'pipeline done!!!'
        }
    }
}
