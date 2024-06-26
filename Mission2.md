GitHub 사용법
===
GitHub란?
---
+ 깃(Git)을 사용하는 프로젝트를 지원
+ 개발자들의 버전 제어 및 협업을 위한 하나의 플랫폼
+ 클라우드를 통해 관리되는 버전 관리 시스템
+ 오픈 소스는 일정 부분 무료로 사용이 가능하나, 대부분 유료 시스템
+ 깃처럼 자체적으로 구축하는 시스템이 아닌, 클라우드를 빌려쓰는 개념
+ 클라우드 서비스기 때문에 다른 사람들과 협업 시 소스코드 공유 가능

Git이란?
---
+ 로컬에서 관리되는 버전 관리 시스템
+ 직접 소스 코드를 수정함으로서 버전을 관리
+ 소스 코드를 효율적으로 관리할 수 있게 해주는 형상 관리 도구
+ 로컬 저장소를 사용하기 때문에, 다른 사람이 나의 작업 내용을 알 수 없음
### 1) Git의 주요 개념들
----
+ **Local** : 사용자의 컴퓨터   
+ **Remote** : 원격 저장소   
+ **Repository(repo, 저장소)** : 프로젝트가 존재하는 저장공간  
+ **branch** : Repsitoy의 공간에서 독립적으로 어떤 작업을 하기 위한 공간    
+ **Commit** : 소스코드의 업데이트를 확정. 확정된 순간의 코드 상태를 메세지와 함께 Git Repo에 저장   
+ **Pull** : 원격저장소의 내용을 로컬저장소에 끌어오는 것   
+ **Push** : Commit한 내용을 원격 저장소에 업로드   
### 2) Git의 주요 명령어들
---
+ **git init** : 깃 초기화
+ **git status** : 깃 저장소 상태 확인
+ **git add** : 커밋에 파일의 변경 사항을 포함
+ **git commit** : 커밋을 생성하고, 변경 사항을 확정 및 반영
+ **git clone** : 기존 소스 코드 다운로드 및 복제
+ **git log** : 나의 커밋 내역에 대해 알고 싶을 때 사용하면 현재 커밋 목록들을 확인 가능
+ **git checkout** : 브랜치에서 브랜치로 이동
+ **git checkout master** : 이전 버전, 변경 전 브랜치에서 다시 현재의 (master) 브랜치로 되돌아 올 수 있다.
+ **git push** : 소스 코드의 변경 사항을 원격 저장소에 반영
+ **git pull** : 원격 저장소의 변경 내용이 현재 디렉토리로 가져와진 뒤 병합
+ **git merge** : 변경 사항 등이 모두 확정되고 난 후, 브랜치들을 병합