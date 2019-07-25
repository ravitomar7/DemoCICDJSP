pipeline {
    agent any

    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                    echo "JAVA_HOME = ${JAVA_HOME}"
                                   '''
            }
        }

        stage ('Build') {
            steps {
                dir("/opt/apache-tomcat-7.0.94/webapps/ravi") {
                sh 'git pull'
                }
               
            }
        }
}
}
