node('nodejs') {
	stage('Checkout') {
		git branch: 'main',
			url: 'https://github.com/victorrafols009/do400-pipelines-control'
	}
	stage('Backend Tests') {
		sh 'node ./backend/test.js'
	}
	stage('Frontend Tests') {
		sh 'node ./frontend/test.js'
	}
}
