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
                echo 'Bridger, Neeebbbbbeeeeeeey'
                echo 'Bridgeeeeeeeeeeeehhhhhhhhey'
             
               
            }
        }
        stage('Descr') {
            steps {
                echo 'Hyuderabad'
                echo 'Suncity'
                echo 'Hyuderabad'
                echo 'Sunciiimiiiiiiiiiity'
              
            }
        }
    }

   post {
        always {
            script {
                def jobName = env.JOB_NAME
                def buildNumber = env.BUILD_NUMBER
                def buildStatus = currentBuild.currentResult

                // Construct the payload as a map
                def payload = [
                    jobName: jobName,
                    buildNumber: buildNumber,
                    status: buildStatus
                ]

                // Convert map to JSON string
                def payloadJson = writeJSON returnText: true, json: payload

                // Send notification
                httpRequest(
                    httpMode: 'POST',
                    url: 'http://<your_server_ip>:3000/webhook',
                    contentType: 'APPLICATION_JSON',
                    requestBody: payloadJson
                )
            }
        }
    }
    
}
