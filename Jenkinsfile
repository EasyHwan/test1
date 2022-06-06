pipeline {
    agent  {
        label "demoAgent"
    } 

    stages {
        stage('Test') {
            steps {
                echo "Test"
            }
        }
    }
    post {
        always{
            echo 'pipeline done'
        }
    }
}
