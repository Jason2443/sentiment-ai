stage('Lint') {
    steps {
        sh '''
        docker run --rm \
        -v "$WORKSPACE":/app \
        -w /app \
        python:3.12-slim \
        /bin/sh -c "pip install flake8 -q && ls -la && ls -la src && flake8 src --max-line-length=100"
        '''
    }
}