pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/punit5670/bookingweb.git'
            }
        }
        stage('Deploy') {
            steps {
                echo "HTML site को deploy कर रहे हैं..."
                sh '''
                  mkdir -p /var/www/html/bookingweb
                  cp -r * /var/www/html/bookingweb/
                '''
            }
        }
    }
}
