pipeline {
    agent any

    stages {
        stage('Información ciudad') {
            steps {
                script {
                    ciudad = 'Madrid'
                    habitantes = '3.223 millones'
                    climaActual = 'Soleado, 25°C'
                    echo "Ciudad actual: ${ciudad}"
                    echo "Habitantes: ${habitantes}"
                    echo "Clima actual: ${climaActual}"
                }
            }
        }

        stage('Comando BAT') {
            steps {
                bat 'ipconfig /flushdns'
            }
        }

        stage('Informar usuario') {
            steps {
                script {
                    usuario = env.USERNAME
                    echo "Usuario que está ejecutando la tarea: ${usuario}"
                }
            }
        }
    }
}
