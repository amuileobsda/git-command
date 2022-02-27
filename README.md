# _CommandGit
✔️ Git _Command
```
$ git branch -> 로컬 branch 확인  
$ git branch -r 서버 branch 확인  
$ git checkout -b 브랜치명 브랜치를 만들고 바로 이동  
$ git branch -d(D) test 브랜치 삭제  
$ git status 현재상태(머지나 추가사항) 확인  
$ git add 경로 에러를 해결하고 추가하여 에러해결  
$ git stash 임시저장  
$ git stash pop 임시저장한파일 불러오기  
$ git remote prune origin 깃랩에서 삭제한거 서버와 동기화  
$ git push origin :브랜치네임 서버에서 삭제하기  
$ git remote  
$ git push origin dev  
$ git config http.postBuffer 104857600 git오류시 해결  
$ git merge --squash dev  
$ git merge --no-ff feature- : 새로운 가지 따서 merge(관리상 용이)  
$ git clone 주소  
$ git remote set-url origin 주소 : gitlap 저장소 변경시 설정  
$ git remote -v : gitlap 저장소 주소 확인  
  
// 고아 브랜치 만드는 방법  
$ git checkout master  
$ git checkout --orphan c_YYMMDD_CAMPAIGNNAME  
$ git rm -rf .  
$ git push origin c_YYMMDD_CAMPAIGNNAME  

// 자주 쓰는 명령어  
$ git remote add origin "주소"  
$ git remote -v  
$ git push -f origin master :원격저장소도 master고 로컬저장소도 master인데 원격저장소에 이력안남을때 로컬에서 강제 푸쉬   
$ git push -u origin master :강제푸쉬   

$ git init : git 생성하기   
$ git clone git_path : 코드가져오기   
$ git checkout branch_name : 브랜치 선택하기   
$ git checkout -t remote_path/branch_name : 원격 브랜치 선택하기   
$ git branch branch_name : 브랜치 생성하기   
$ git branch -r : 원격 브랜치 목록보기   
$ git branch -a : 로컬 브랜치 목록보기   
$ git branch -m branch_name change_branch_name : 브랜치 이름 바꾸기   
$ git branch -d branch_name : 브랜치 삭제하기   
$ git push remote_name — delete branch_name : 원격 브랜치 삭제하기 ( git push origin — delete gh-pages )   
$ git add file_path : 수정한 코드 선택하기 ( git add * )   
$ git commit -m “commit_description” : 선택한 코드 설명 적기 ( git commit -m “내용”)   
$ git push romote_name branch_name : add하고 commit한 코드 git server에 보내기 (git push origin master)   
$ git pull : git서버에서 최신 코드 받아와 merge 하기   
$ git fetch : git서버에서 최신 코드 받아오기   
$ git reset — hard HEAD^ : commit한 이전 코드 취소하기   
$ git reset — soft HEAD^ : 코드는 살리고 commit만 취소하기   
$ git reset — merge : merge 취소하기   
$ git reset — hard HEAD && git pull : git 코드 강제로 모두 받아오기   
$ git config — global user.name “user_name ” : git 계정Name 변경하기   
$ git config — global user.email “user_email” : git 계정Mail변경하기   
$ git stash / git stash save “description” : 작업코드 임시저장하고 브랜치 바꾸기   
$ git stash pop : 마지막으로 임시저장한 작업코드 가져오기   
$ git branch — set-upstream-to=remote_path/branch_name : git pull no tracking info 에러해결   

$ git cherry-pick <commit_hash_1> <commit_hash_2> ... : 일정 범위의 커밋을 가져오는 방법   

$ git checkout -b feature/test   
feature/test > git add .   
feature/test > git commit -m 'fix typo'   
$ git rebase -i @~3   (참고: -i는 --interactive 옵션이고, @~3은 최근 3개의 commit을 rebase하겠다는 뜻이다 HEAD~3과 같은 뜻이다.)   

$ git ls-files | xargs cat | wc -l   
$ git ls-files | xargs wc -l   
$ wc -l `find . -name '*.json'`   
$ find . -name '*.js' | xargs wc -l   

// 로그확인
$ git log -p   
$ git log -p README.md   
$ git log --oneline   
$ git log --name-only   


// 빠르게 쓰는 명령어   
$ git remote add "저장소명" "url"   
$ git remote -v   
$ git pull 저장소명 +master   
$ git push 저장소명 +master   
$ git remote rm 저장소명   
```
