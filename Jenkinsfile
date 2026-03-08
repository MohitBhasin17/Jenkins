pipeline {
    agent any

    triggers {
        // Listens for the GitHub Webhook signal
        githubPush() 
        // Backup: Checks for changes every 5 minutes
        cron('H/5 * * * *') 
    }

    stages {
        stage('Build') {
            steps {
                echo 'Build triggered by GitHub push or cron schedule'
            }
        }
    }
}






