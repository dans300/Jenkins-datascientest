pipeline {
    agent any // means any agent
    stages {
        stage('Greeting') {
            steps {
                echo 'Hello Datascientest'
            }
        }
    }
}
agent {
  docker {
    image 'gradle:6.9-alpine'
    label 'datascientest-gradle'
    args  '-v /tmp:/tmp'
  }
}
