pipeline{
    agent any
    tools {
        jdk "Jdk17"
        maven "Maven3"
    }
    
    stages {
        stage("Cleaning workspace..."){
            steps {
                 cleanWs()
            }
        }

        stage("Checkout from SCM..."){
            steps {
                git branch: "master",  url:"https://github.com/dmancloud/complete-prodcution-e2e-pipeline.git"
            }
        }

        stage ("Build application..."){
            steps {
                sh "mvn clean package"
            }
        }

        stage ("Run test"){
            steps {
                sh "mvn test"
            }
        }

    }
    
}
