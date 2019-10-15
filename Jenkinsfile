pipeline{
    agent any
    stages{
        stage('Git Checkout'){
            steps{
                git url: 'https://github.com/9492678901/mongodb-realtime.git'
            }
        }
        
        stage('Dev Deploy'){
            steps{
                sh "ansible-playbook -i dev.invenory mongodb.yml"
            }
        }
        
    }
}
