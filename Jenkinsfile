pipeline {
    agent {
        node {
            label 'built-in' // Use Jenkins' built-in node
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Pavan kalyan bakkani'
                echo 'Bridger, Neeeeeeeeeeeeeeeey'
                echo 'Bridger, Neeebbbbbbeeeeeeeeeeeeey'
                echo 'Bridger, Neeeeeeeeeeeeeeehhhhhhhhhhhhhhhhhey'
                sh 'exit 1'
               
            }
        }
        stage('Descr') {
            steps {
                echo 'Hyuderabad'
                echo 'Suncity'
                echo 'Hyuderabad'
                echo 'Sunciiimmmmmmmiiiiiiiiiiiiiiiiiiity'
                sh 'exit 1'
            }
        }
    }

    post {
        success {
            script {
               
                    echo "ABD"
                }
            }
        }
        failure{
            echo 'build has failed'
    }
}
