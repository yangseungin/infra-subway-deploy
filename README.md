<p align="center">
    <img width="200px;" src="https://raw.githubusercontent.com/woowacourse/atdd-subway-admin-frontend/master/images/main_logo.png"/>
</p>
<p align="center">
  <img alt="npm" src="https://img.shields.io/badge/npm-%3E%3D%205.5.0-blue">
  <img alt="node" src="https://img.shields.io/badge/node-%3E%3D%209.3.0-blue">
  <a href="https://edu.nextstep.camp/c/R89PYi5H" alt="nextstep atdd">
    <img alt="Website" src="https://img.shields.io/website?url=https%3A%2F%2Fedu.nextstep.camp%2Fc%2FR89PYi5H">
  </a>
  <img alt="GitHub" src="https://img.shields.io/github/license/next-step/atdd-subway-service">
</p>

<br>

# 인프라공방 샘플 서비스 - 지하철 노선도
## 배운점
AWS를 사용해서 망 분리하기, 통신 확인하기, 도커에 대한 이해 
- VPC, Subnet 생성
- Reverse Proxy 구성
- 배포스크립트 작성하기
- 배포스크립트 작성하기
- 설정파일을 나누고 운영환경과 개발환경 나누기

## 느낀점
- 사이드 프로젝트를 진행하면서도 AWS를 사용해봤지만 VPC나 Subnet, 망분리에 대해 구체적으로 사용해본 적이 없었는데 실제로 서비스를 해본다는 가정하에 구성해볼 수 있어서 좋았다.








<br>

## 🚀 Getting Started

### Install
#### npm 설치
```
cd frontend
npm install
```
> `frontend` 디렉토리에서 수행해야 합니다.

### Usage
#### webpack server 구동
```
npm run dev
```
#### application 구동
```
./gradlew clean build
```
<br>

## 미션

* 미션 진행 후에 아래 질문의 답을 README.md 파일에 작성하여 PR을 보내주세요.

### 0단계 - pem 키 생성하기

1. 서버에 접속을 위한 pem키를 [구글드라이브](https://drive.google.com/drive/folders/1dZiCUwNeH1LMglp8dyTqqsL1b2yBnzd1?usp=sharing)에 업로드해주세요

2. 업로드한 pem키는 무엇인가요.
- KEY-yangseungin.pem

### 1단계 - 망 구성하기
1. 구성한 망의 서브넷 대역을 알려주세요
- 대역 :
    - vpc : 192.168.123.0/24
    - yangseungin-public1 : 192.168.123.0/26
    - yangseungin-public2 : 192.168.123.64/26
    - yangseungin-private : 192.168.123.128/27
    - yangseungin-management : 192.168.123.160/27

2. 배포한 서비스의 공인 IP(혹은 URL)를 알려주세요
- IP : 54.180.156.102:8080
- URL : http://yang-infra-subway.p-e.kr:8080



---

### 2단계 - 배포하기
1. TLS가 적용된 URL을 알려주세요

- URL : https://https://yang-infra-subway.p-e.kr/

요구사항  
- [x] 운영 환경 구성하기
  - [x] 웹 애플리케이션 앞단에 Reverse Proxy 구성하기
    - [x] 외부망에 Nginx로 Reverse Proxy를 구성
    - [x] Reverse Proxy에 TLS 설정
  - [x] 운영 데이터베이스 구성하기
- [x] 개발 환경 구성하기
  - [x] 설정 파일 나누기

---

### 3단계 - 배포 스크립트 작성하기

1. 작성한 배포 스크립트를 공유해주세요.
 deploy.sh
2. 

