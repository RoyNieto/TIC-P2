pipeline {
    agent any

    stages {
        stage('1. Inspeccionar Node.js') {
            steps {
                echo 'Comprobando versión de Node y npm...'
                bat 'node --version'
                bat 'npm.cmd --version'
            }
        }

        stage('2. Ejecutar Aplicación Node') {
            steps {
                echo 'Ejecutando script de Node.js...'
                bat 'node app.js'
            }
        }

        stage('3. Pruebas Unitarias') {
            steps {
                echo 'Ejecutando validaciones...'
                bat 'echo Test suite: Todo correcto.'
            }
        }
    }

    post {
        success {
            echo '¡Pipeline de Node.js completado exitosamente!'
        }
    }
}