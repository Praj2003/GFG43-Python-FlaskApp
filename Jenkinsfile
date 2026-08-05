pipeline {  //pipeline where all stages are presen
    agent {label "worker1" }
    stages { //collection of stages
        stage("Deploy the app in dev env"){ // job1 first job
            steps {
                sh 'docker pull prajval2003/gfg43cicd:latest'
                sh 'docker rm -f webapp'
                sh 'docker run -dit --name webapp -p 80:80 prajval2003/gfg43cicd:latest'
            }
        }
    }
}