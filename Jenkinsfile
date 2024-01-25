pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                sh 'rm -rf jenkin_backup'
                sh 'git https://github.com/sudhasanshi/jenkin_backup.git'
            }
        }

        stage('backup') {
            steps {
                sh ' cp -R /var/lib/jenkins/ /jenkin_backup/backup_files
            }
        }
		
	
