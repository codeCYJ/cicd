pipeline {

     agent any

     stages {

        stage("Build") {

            steps {

                sh "sudo npm install"

                sh "sudo npm run build"

            }

        }

        stage("Deploy") {

            steps {

                 script {

                    sh 'sudo chmod +x ./script/deploy.sh'

                    sh 'sudo ./script/deploy.sh'

                }

            }

        }

    }

}