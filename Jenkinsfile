pipeline{
agent any
   stages{
        stage('Update Local'){
            steps{
                sh "sudo apt update -y"

            }

        }

        stage('Install Nginx'){
            steps{
                sh "sudo echo 'installation of nginx'"
                sh 'sudo apt install nginx -y'
            }

        }

        stage('Make file'){
            steps{
               sh 'sudo echo "Welocme to young minds" > index.html' 
                sh 'sudo mv index.html /var/www/html/index.html'
            }

        }

        stage('Start Service'){
            steps{
                sh 'sudo systemctl start nginx'
            }

        }


}

}
