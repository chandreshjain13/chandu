pipeline {
    agent any
    tools {
        maven 'maven3'
        jdk 'java8'
    }
stages {
    stage('clone') {
        steps {
            git credentialsId: '0df6070c-2ff1-4606-b730-b1b67d13d4a0', url: 'https://github.com/chandreshjain13/chandu.git'
            
        }
    }
    stage ('Build') {
        steps {
            sh 'mvn clean package'
        }
    }
    stage ('deploy') {
        steps {
            sh "echo deploy success"
        }
    }
        
    }

}
