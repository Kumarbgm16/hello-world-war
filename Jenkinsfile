pipeline {
    agent { label 'java' } 
    stages {
        stage('checkout') {
            steps {
                sh 'git clone https://github.com/Kumarbgm16/hello-world-war.git'
            }
        }

stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }
stage('deploy') {
steps {
sh 'cp /home/slave-1/workspace/t3/target/hello-world-war-1.0.0.war /opt/apache-tomcat-9.0.62/webapps'
    }
}
}
}
