pipeline {
    agent{
        label "ec2"
    }

    stages {
        stage("Deploy in PROD"){
            steps {
                sh "docker rm -f webos"
                sh "docker run -dit --name webos -p 81:80 jinny1/gfgflask18"
            }
        }
}
}