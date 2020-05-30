# Guider Web

### Setting
Set publicPath to the IP of your web server
```shell script
$ vi ./django_vue/vue.config.js
```
This is Example. Change 211.10.52.1 to Your Server`s Public IP!
```js
module.exports = {
  publicPath: 'http://211.10.52.1:8080/', 
  outputDir: "../static",
  ....
}
```

### Install Python Dependencies
```shell script
$ pip3 install virtualenv
```
```shell script
$ virtualenv venv 
```
```shell script
$ source ./venv/bin/activate
```
```sh
$ pip3 install -r requirements.txt
```

### Build Frontend Codes
```sh
$ cd ./django_vue/ && npm install && npm run build && cd ..
```

### Run
Run frontend
```
$ cd ./django_vue/ && npm run serve
```
Run backend
```sh
$ python3 manage.py runserver 0.0.0.0:8000
```