pipeline {
    agent { label "linux" }
    stages {
        stage('ansible') {
            steps {
                script {
                    ansiblePlaybook (
                        playbook: 'main.yml',
                        inventory: 'inventory.yml',
                        colorized: true
                    )
                }
            }
        }
    }
}