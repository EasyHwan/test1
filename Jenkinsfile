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
            def dateFormat = new SimpleDateFormat("yyMMddHHmm")
            def date = new Date()
            def TODAY = dateFormat.format(date)
    
            sh "echo ${TODAY}"
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
