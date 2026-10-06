pipeline{
    agent any
    stages{
        stage("Clone repo"){
            steps{
                git url: 'https://github.com/nabiswavalencia/java-todo', branch: 'master'
            }
        }
    stage("Build code"){
        steps{
            sh './gradlew build'
        }
    }
    stage("Test Code"){
        steps{
            sh "./gradlew test"
        }
    }
    }
}