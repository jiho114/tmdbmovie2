# 환경변수 .env

.env는 src같은 위치에 생성 (최상위 폴더) \
.env 파일 안에 REACT_APP_API_TMDB_KEY="API _KEY" \
주의점 : 맨 뒤에 세미콜론 쓰지 않기 \

## .gitignore 파일에 .env 올리지 않기 .env 작성

gitignore에 있는 파일들은 깃에 올리지 말아야 할 파일들을 작성함 \

## API KEY 사용
변수 const api (변수명) = process.env.REACT_APP_API_TMDB_KEY;
### 깃 배포하기 

packge.json 수정하기 \
패키지 제이슨 하단에 홈페이지 주소 삽입 \
"homepage": "https://jiho114.github.io/tmdb1" 깃 허브 홈페이지 주소\ 
(https://jiho114.github.io/tmdb1) \

script 수정 \
"predeploy": "npm run build", \
"deploy": "gh-pages -d build" \

깃저장소 업로드

### 터미널에서 gh-pages 설치하기
npm i gh-pages 명령어

### 깃허브 저장소 다시 확인하기
git remote -v \

### 깃허브 배포하기
npm run deploy

