pipeline {
    agent  {
        label "demoAgent"
    } 

    stages {
        stage('Test') {
            steps {
                echo "Testing"
            }
        }
    }
    post {
        always{
            echo 'pipeline done'
        }
    }
}
