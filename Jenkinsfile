pipeline {
    agent { label 'jdk11-mvn3.8.4' }
    triggers {
        cron('45 23 * * 1-5')
<<<<<<< HEAD
        pollSCM('*/5 * * * *')
=======
        pollSCM('*/5 * * * *)
>>>>>>> ce06148e63fca5714d831a4cfe99c1230ecfe4c6
    }
    stages {
        stage('scm') {
            steps {
                git 'https://github.com/arvindmahat/java11-examples.git'
            }
        }
        stage ('build') {
            steps {
                sh '/usr/local/apache-maven-3.8.4/bin/mvn clean package'
            }
        }
    }
}
