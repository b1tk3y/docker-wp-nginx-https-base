# docker-wp-nginx-https-base
NGINX로 서브도메인을 이용한 웹사이트 운영 예시코드를 간단히 설명한다.

## 예시 도메인
- example.com(www.example.com으로 redirect)
- www.example.com
- blog.example.com
- mirror.example.com

## 스택
- Docker(compose)
- WordPress
- MariaDB
- NGINX
- Letsencrypt

## letsencrypt
먼저 `init-letsencrypt.sh`에서 `domains`와 `email`을 변경한다. 그리고나서 아래 명령을 실행한다.

1. `make up` 명령을 실행한다.
2. `./init-letsencrypt.sh`를 실행한다.
3. nginx가 재시작 될 때까지 기다린다.