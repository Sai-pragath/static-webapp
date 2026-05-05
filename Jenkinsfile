pipeline {
agent any

```
stages {

    stage('Checkout') {
        steps {
            git 'https://github.com/YOUR-USERNAME/static-webapp.git'
        }
    }

    stage('Build') {
        steps {
            echo "No build needed for static app"
        }
    }

    stage('Deploy') {
        steps {
            sh '''
                echo "Deploying static site..."

                rm -rf /var/www/html/*
                cp -r * /var/www/html/

                echo "Deployment complete!"
            '''
        }
    }
}
```

}
