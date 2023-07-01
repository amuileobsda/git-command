# Git

- [Git Command](#git-command)
- [Branch 관련 명령어](#branch-관련-명령어)
- [상태 확인 및 변경 명령어](#상태-확인-및-변경-명령어)
- [원격 저장소 관련 명령어](#원격-저장소-관련-명령어)
- [코드 관리 명령어](#코드-관리-명령어)
- [임시 저장 관련 명령어](#임시-저장-관련-명령어)
- [이력 및 로그 관련 명령어](#이력-및-로그-관련-명령어)
- [일반적인 명령어](#일반적인-명령어)
- [빠르게 쓰는 명령어](#빠르게-쓰는-명령어)

## Git Command

### Branch 관련 명령어
```
$git branch                       # 로컬 브랜치 확인
$git branch -r                    # 원격 브랜치 확인
$git checkout -b 브랜치명          # 브랜치 생성 후 이동
$git branch -d(D) test            # 브랜치 삭제
```
### 상태 확인 및 변경 명령어
```
$git status                        # 현재 상태 확인
$git add 경로                      # 변경 내용 추가 및 에러 해결
```
### 원격 저장소 관련 명령어
```
$git remote                         # 리모트 저장소 확인
$git push origin :브랜치명           # 서버에서 브랜치 삭제
$git remote prune origin            # 깃랩에서 삭제한 것 서버와 동기화
$git push origin dev                # dev 브랜치로 푸시
$git remote add origin "주소"       # 원격 저장소 추가
$git remote -v                      # 원격 저장소 목록 확인
$git remote rm 저장소명              # 원격 저장소 제거
```
### 코드 관리 명령어
```
$git merge --squash dev            # dev 브랜치와 squash로 병합
$git merge --no-ff feature-        # 새로운 가지 따서 merge (관리상 용이)
$git clone 주소                    # 주소에서 코드 가져오기
$git remote set-url origin 주소    # GitLab 저장소 주소 변경 설정
```
### 임시 저장 관련 명령어
```
$git stash                         # 변경 내용 임시 저장
$git stash pop                     # 최근에 임시 저장한 파일 불러오기
```
### 이력 및 로그 관련 명령어
```
$git log -p                        # 모든 커밋 로그 및 변경 내용 확인
$git log --oneline                 # 커밋 로그를 한 줄로 확인
$git log --name-only               # 변경된 파일 목록만 확인
$git log --graph                   # 커밋 그래프 확인
```
### 일반적인 명령어
```
$git init                                    # Git 생성하기
$git add file_path                           # 수정한 코드 선택하기
$git commit -m "commit_description"          # 선택한 코드 설명 적기
$git push origin branch_name                 # add하고 commit한 코드를 Git 서버에 보내기
$git pull                                    # Git 서버에서 최신 코드를 받아와서 merge하기
$git config --global user.name "user_name"    # Git 계정 이름 변경하기
$git config --global user.email "user_email"  # Git 계정 이메일 변경하기
```
### 빠르게 쓰는 명령어
```
$git remote rm "저장소명"
$git init
$git remote add origin "저장소명" "url"
$git remote -v
$git pull "저장소명" +master
$git push "저장소명" +master
$git push -u origin master                    #강제푸쉬
```
