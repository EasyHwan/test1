import java.text.SimpleDateFormat

import java.text.SimpleDateFormat
pipeline {
    agent  {
        label "demoAgent"
    } 
    
    stages {
        stage('Prepare Today Date') {
            steps {
                 script {
                    def dateFormat = new SimpleDateFormat("yyyyMMddhhmm")
                    def date = new Date()
                
                    today = dateFormat.format(date)                
                    
                }                
            } 
        }
        stage('Print Today Date') {
            steps {
                  echo today
            } 
        }
}
}
