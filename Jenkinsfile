pipeline {
    agent any

    stages {
        stage('Clonar Repositorio con pipelines') {
            steps {
                script {
                    // Paso para clonar el repositorio de GitHub
                    git branch: 'main', url: 'https://github.com/Lauty04/WEBapache.git'
                }
            }
        }

        // Agrega más etapas según sea necesario
    }
}
