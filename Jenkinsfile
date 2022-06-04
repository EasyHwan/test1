import java.text.SimpleDateFormat
pipeline {
    agent  {
        label "demoAgent"
    } 

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                def dateFormat = new SimpleDateFormat("yyyyMMddhhmm")
                def date = new Date()
                today = dateFormat.format(date)
                echo today
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
            echo 'pipeline done'
        }
    }
}
