def data = "test"
pipeline {
    agent any
    stages {
        stage("read file") {
            steps {
                //sh "touch sample.text"
                echo "${WORKSPACE}"
                script {
                    data = readFile(file: "${WORKSPACE}/sample.txt")
                }
                   println(data)
                
                }
            }
        }
    }
