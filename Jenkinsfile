podTemplate(containers: [
    containerTemplate(name: 'apache-container', image: 'httpd', command: 'sleep', args: '99d')
]) {
node(POD_LABEL) {
            container('apache') {
                stage('run apache container') {
                    sh 'echo my name is sagore'
                }
            }
        }
}
