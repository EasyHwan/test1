pipeline {
    agent  {
        label "demoAgent"
    } 

    stages {
        stage('Test') {
            steps {
                echo "202206061121"
            }
        }
    }
    post {
        always{
            echo 'pipeline done'
        }
    }
}
