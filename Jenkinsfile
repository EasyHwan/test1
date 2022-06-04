pipeline {
    agent  {
        label "demoAgent"
    } 

    stages {
        stage('Test') {
            steps {
                echo "202206041122"
            }
        }
    }
    post {
        always{
            echo 'pipeline done'
        }
    }
}
