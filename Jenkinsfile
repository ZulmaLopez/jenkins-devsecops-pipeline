pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compilando el proyecto...'
            }
        }
        stage('Test') {
            steps {
                echo 'Ejecutando pruebas automatizadas...'
            }
        }
        stage('SCA - Dependency Check') {
            steps {
                echo 'Analizando dependencias vulnerables...'
            }
        }
        stage('SAST - Static Analysis') {
            steps {
                echo 'Ejecutando análisis estático de código...'
            }
        }
        stage('Security Gate') {
            steps {
                echo 'Verificando criterios de seguridad...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Desplegando aplicación...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completado exitosamente.'
        }
        failure {
            echo 'Pipeline falló. Revisar logs.'
        }
    }
}