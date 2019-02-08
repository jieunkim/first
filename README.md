# first
최초 flask app 소스 관리

배포 관련 사항
deploy.json : 도메인, 아이피 등 정보
              형식이 json이라서 주석 불가 (주석쓰면 오류남)
fabfile.py : 페븩 작업 내용 기술
fabfile_comment.py : 주석 버전
wsgi.py : entry 파일, 서버구동시 시작점
requirements.txt : 서버 구동시 필요한 모듈을 기술 (버전 포함)

# 서버 로그 확인
리눅스 명령
> tail -f 로그파일명 => 이 파일이 변환되는 것을
  실시간적으로 읽어서 출력해라
접속 로그 (파이썬 로그)
> tail -f /var/log/apache2/access.log
> ctrl + c
에러 로그 (500에러 발생시, internal server error)
> tail -f /var/log/apache2/error.log
> ctrl + c