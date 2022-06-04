pipeline {
    agent  {
        label "demoAgent"
    } 

    stages {
        stage('Test') {
            steps {
                build '202206041122'
            }
        }
    }
    post {
        always{
            echo 'pipeline done'
        }
    }
}
