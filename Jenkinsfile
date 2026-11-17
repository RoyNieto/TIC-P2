pipeline {
    agent any

    stages {
        stage('1. Inspeccionar') {
            steps {
                echo "Ejecutando pipeline para la rama ${env.GIT_BRANCH}..."
                bat 'git --version'
            }
        }

        stage('2. Compilación') {
            steps {
                echo 'Simulando compilación del código...'
                bat 'echo Compilación exitosa.'
            }
        }

        stage('3. Pruebas') {
            steps {
                echo 'Simulando pruebas automatizadas...'
                bat 'echo Pruebas: 100% pasadas.'
            }
        }
    }

    post {
        success {
            echo '¡Pipeline finalizado con éxito tras el push!'
        }
    }
}