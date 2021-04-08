pipeline {
    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'about person')

        text(name: 'ABOUT', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'AGREE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['JAVA', 'JavaScript', 'Python'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.PERSON}"

                echo "about: ${params.ABOUT}"

                echo "AGREE: ${params.AGREE}"

                echo "Choice: ${params.CHOICE}"

                echo "Password: ${params.PASSWORD}"
            }
        }
    }
}
