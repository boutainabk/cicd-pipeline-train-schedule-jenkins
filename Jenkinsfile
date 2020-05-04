pipeline {
    agent any
    stages {
        stage('Build image') {
            steps {
                withDockerRegistry([ credentialsId: "dockervm12", url: "" ]) {
                // following commands will be executed within logged docker registry
                   sh 'docker push dockervm12/linuxaclab:tag'
                }
            }
        }
    }
}
