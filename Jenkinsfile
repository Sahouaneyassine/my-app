pipeline {
    agent any

    tools {
        maven "maven"
        jdk "jdk11"
    }

    stages {
        stage('Initialize'){
            steps{
                //echo "PATH = ${M2_HOME}/bin:${PATH}"
                echo "M2_HOME = /usr/share/maven"
            }
        }
        stage('Build') {
            steps {
                dir("/var/lib/jenkins/workspace/my-app") {
                sh 'mvn -B -DskipTests clean package'
                }
            
            }
        }
     }

}
