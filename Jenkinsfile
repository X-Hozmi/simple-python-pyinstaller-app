node {
    docker.image('python:3.8').inside {
        stage('Build') {
            sh 'python -m py_compile /var/jenkins_home/workspace/submission-cicd-pipeline-abdil_haidar/sources/add2vals.py /var/jenkins_home/workspace/submission-cicd-pipeline-abdil_haidar/sources/calc.py'
            stash name: 'compiled-results', includes: 'sources/*.py*'
        }
    }
}
