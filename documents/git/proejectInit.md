# Project Init
### GitHub을 이용하여 신규 프로젝트의 Git을 연결할 떄
1. [GitHub] GitHub에서 신규 프로젝트 Repository 생성
1. [Local] Local에서 신규 GitHub 프로젝트와 연결할 새로운 프로젝트 생성
1. [Local] `git init`으로 git 설정 추가
1. [GitHub] GitHub에서 생성한 프로젝트의 URL 복사
1. [Local] `git remote add origin "GitHub URL"`으로 github origin 정보 추가
1. [Local] 프로젝트 구성을 위한 작업
1. [Local] 작업 내역에 대해 `git add 파일명` or `git add .`
1. [Local] `git commit -m 설명`으로 해당 내용 commit
1. [Local] `git push origin master`로 origin에 있는 master 브랜치에 작업 내역을 Push
1. [GitHub] Repository에서 Push된 내역 확인
