pipeline {
    agent  {
        label "demoAgent"
    } 

    stages {
        stage('Test') {
            steps {
                build 'SeleniumMaven'
            }
        }
    }
    post {
        always{
            echo 'pipeline done'
        }
    }
}
