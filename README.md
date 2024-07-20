### `post README.md`

#### `judy-community-backend-post`

# Judy Community Post Backend

게시물 관리 및 관련 작업을 처리하는 백엔드 서비스입니다.

## 구조

```
judy-community-backend-post/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── judycorp/
|   │   │           └── post/
│   │   │               ├── config/
│   │   │               ├── controller/
│   │   │               ├── dto/
│   │   │               ├── entity/
│   │   │               ├── exception/
│   │   │               ├── repository/
│   │   │               ├── service/
│   │   │               └── ApplicationPost.java
│   ├── resources/
│   │   └── application.properties
├── Dockerfile
├── build.gradle.kts
└── settings.gradle.kts
└── .github/
    └── workflows/
        └── ci-cd.yml
```

## 기능

- 게시물 생성
- 게시물 조회
- 게시물 수정 및 삭제

## 설치 및 실행

### 사전 요구 사항

- [Docker](https://www.docker.com/get-started)
- [JDK 17](https://adoptopenjdk.net/)

### Docker 이미지 빌드 및 실행

```bash
./gradlew build
docker build -t your_dockerhub_username/judy-community-backend-post .
docker run -p 8083:8080 your_dockerhub_username/judy-community-backend-post
```
