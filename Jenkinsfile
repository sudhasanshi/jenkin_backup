pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                sh 'rm -rf jenkin_backup'
                sh 'git clone https://github.com/sudhasanshi/jenkin_backup.git'
            }
        }

        stage('backup') {
            steps {
                sh ' rsync /var/lib/jenkins/workspace/jenkin-backup /jenkin_backup/backup_files/'
            }
        }
		
	}
}
