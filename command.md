# 명령어

- docker (Management Command) Command
- `docker version`
  - 버전 및 상태 확인
- `docker info`
  - 플러그인, 시스템 상세 정보 확인
- `docker --help`
  - 명령어 메뉴얼 확인
- `docker run (실행옵션) 이미지명`
  - 컨테이너 실행
  - ex) docker run -p 80:80 --name hellonginx nginx
- `docker rm 컨테이너명/ID`
  - 컨테이너 삭제
  - ex) docker rm hellonginx

## 컨테이너 삭제

[MacOS]
docker rm -f $(docker ps -aq)

[Windows]
docker ps -aq | ForEach-Object {docker rm -f $\_}
(PowerShell에서 실행하셔야 합니다.)
