node {
    docker.image('python:3.8').inside {
        stage('Build') {
            sh 'python -m py_compile sources/add2vals.py sources/calc.py'
            stash name: 'compiled-results', includes: 'sources/*.py*'
        }
    }
}
