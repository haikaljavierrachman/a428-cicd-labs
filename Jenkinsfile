node {
    docker.image('node:16-buster-slim').inside('-p 3300:3300') {
         stage ('Build') {
             sh 'npm install'
         }

         stage ('Test') {
             sh './jenkins/scripts/test.sh'
         }
    }
}
