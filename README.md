# KsMf skeleton Proxy App

## Install
- git clone https://github.com/ameksike/ksmf-skeleton-proxy.git
- mv ./ksmf-skeleton-proxy ./myproject   #... rename project folder
- cd myproject
- npm install 

## Develop
- npm run client:watch
- npm run dev



## Skeleton
Below you can see the general structure of a full stack project:
```
+ client/
+ server/
- LICENSE
- README.md
- package.json
- .gitignore
- .env
```

- **client:** This directory contains a classic application based on technologies such as Angular, React, VueJs, etc. For more information see [client description](https://github.com/ameksike/ksmf-skeleton-proxy/tree/main/client).
- **server:** This directory contains the source code that runs on the server side, it is usually associated with the web API (database access, remote endpoint access, business logic, etc.)
- **LICENSE:** Product license description file
- **package.json:** The package. json file is the heart of any Node project. It records important metadata about a project which is required before publishing to NPM, and also defines functional attributes of a project that npm uses to install dependencies, run scripts, and identify the entry point to our package.
- **.gitignore:** The . gitignore file tells Git which files to ignore when committing your project to the GitHub repository. gitignore is located in the root directory of your repo. The .gitignore file itself is a plain text document.
- **.env:** A . env file is a text file containing key value pairs of all the environment variables required by your application. This file is included with your project locally but not saved to source control so that you aren't putting potentially sensitive information at risk.

## Docker: Building your own Image 
- docker build -t ksmf-skeleton-proxy .
- docker images 

## Docker: Run image  
- docker run --name myapp --env APPNAME=myapp_v1.0.1 -it -dp 3333:3005 ksmf-skeleton-proxy 
- docker ps -a
- http://localhost:3333
- http://localhost:3333/api/v1/profile
- docker exec -it myapp bash 
- docker stop myapp

## Docker Compose: Building your own image 
- docker-compose build
- docker images

## Docker Compose: Run your own image  
- docker-compose up -d
- http://localhost:5003/api/v1/security/oauth/option
- docker-compose stop

## Server Info 
```json
{
	"origin": {
		"agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:96.0) Gecko/20100101 Firefox/96.0",
		"host": "::1",
		"port": 53999
		"token": "Basic dG9ueTphYmNkLTEyMzQ="
		"user": {
			"username": "tony", 
			"name": "Mr. Tony"
		}
	},
	"destination": {
		"url": "www.youtube.com:443",
		"hostname": "www.youtube.com",
		"href": "//www.youtube.com:443",
		"host": "www.youtube.com:443",
		"port": "443",
		"auth": null,
		"hash": null,
		"path": null,
		"pathname": null,
		"protocol": null,
		"query": null,
		"search": null,
		"slashes": true
	}
}
```

