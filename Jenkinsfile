pipeline {
    agent any

    stages {
        stage('Read Instance IP') {
            steps {
                script {
                    env.INSTANCE_IP = sh(
                        script: "cat ip.txt",
                        returnStdout: true
                    ).trim()
                }
                echo "Captured Instance IP is: ${env.INSTANCE_IP}"
            }
        }
    }
}
