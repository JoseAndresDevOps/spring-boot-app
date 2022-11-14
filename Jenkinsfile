pipeline{
    agent{
        label "Nodojava"
    }    stages{
        stage("test"){
            steps{
                sh "mvn test"
            }
        }
        stage("build"){
            steps{
                sh "mvn clean package -DskipTest"
            }
        }
    }
}
