pipeline {
    agent any

    stages {
        stage('Clonar Repositorio con pipelines') {
            steps {
                script {
                    git branch: 'main', url: 'https://github.com/Lauty04/WEBapache.git', 
                        refspec: '+refs/heads/*:refs/remotes/origin/*'
                }
            }
        }

        // Agrega más etapas según sea necesario
    }
}
