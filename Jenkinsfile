pipeline {
    agent {
    	node {
        label "Nodojava"
        }
    }    
    
    stages{
        stage("test"){
            steps{
                sh "mvn test"
                jacoco()
                junit "target/surefire-reports/*.xml"
            }
        }
        stage("build"){
            steps{
                sh "mvn clean package -DskipTest"
            }
        }
    }
}
