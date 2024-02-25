# Nginx-Basic 
Nginx의 기본 설정을 가이드하기 위한 샘플 예제입니다. 

## Prerequisite 
1. 실습할 PC에 도커 런타임이 설치되어 있어야 합니다. 
2. `docker build`, `docker run` 등 도커 관련 기본 명령어를 다룰 수 있어야 합니다. 

## How to Run 
도커 빌드 및 Nginx 실행 
```sh 
$ git clone git@github.com:sqlpro/nginx-basic.git && cd nginx-basic
$ docker build -t my-nginx . 
$ docker run -p 8080:80 -d --name nginx my-nginx:latest

```

실행 결과 확인 
```sh
$ curl -XGET localhost:8080 

<h1> Hello NginX! </h1>

```

