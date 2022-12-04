# 1. add
**git add** 명령어를 사용하면 현재 작업 디렉토리에 있는 모든 또는 일부 **변경 내용을 스테이징 영역으로 이동**시킬 수 있다.

* ```$ git add <파일/디렉토리 경로>```   
작업 디렉토리의 변경 내용의 일부만 스테이징 영역에 넘기고 싶을 때

* ```$ git add .```   
현재 디렉토리의 모든 변경 내용을 스테이징 영역으로 넘기고 싶을 때

* ```$ git add –A```   
작업 디렉토리 내의 모든 변경 내용을 모두 스테이징 영역으로 넘기고 싶을 때

```
$ git add –A는 작업 디렉토리 어디에 위치하든 항상 동일하게 모든 변경 내용을 스테이징으로 넘기고, 
$ git add 은 명령어를 실행한 디렉토리 이하에서 발생한 변경 내용만 포함한다.
```

<br>

# 2. commit
보통 **git add '파일' -> git commit -> vim 모드에서 버전의 커밋 메시지를 작성**의 순서로 커밋한다.
하지만 커밋 메시지 작성 작업을 명령창에서 바로 할 수 있는 commit 옵션들이 있다.

* ```$ git commit –m "커밋 메시지“```   
commit에서 vim을 들어가 메시지로 작성하는 작업 대신 바로 명령창에서 커밋 메시지를 작성

* ```$ git commit –a```   
별도의 add 명령어를 사용하지 않고 수정된 파일에 대해 add, commit을 한번에 수행   
(단, 한번도 add되지 않은 파일은 따로 작업해 줘야 한다.)

* ```$ git commit –am "커밋 메시지“```   
수정된 파일에 대해 add와 commit을 한 번에 수행

* ```$ git commit —amend```   
최근 커밋을 수정   


<br>

# 3. log
**git log** 명령어로 커밋 기록을 조회. 지금까지의 커밋 기록들이 쭉 출력되며, 가장 위에 나오는 내역이 가장 최근 내역임을 알 수 있다.

* `$ git log`   
커밋 이력 상세 조회

* `$ git log —oneline`      
커밋 이력 중 커밋 ID와 타이틀 메시지만 조회

* `$ git log --oneline --graph`      
commit/merge 등의 log를 그래프의 형태로 조회

* `$ git log --oneline --graph --all`   
모든 브랜치의 log를 그래프의 형태로 조회

* `$ git log ––pretty`   
확장 옵션을 사용하여 여러가지 형태로 표현 가능

<br>

# 4. show
* `$ git show`   
가장 최근의 커밋의 파일에 대한 자세한 정보

* `$ git show head`   
HEAD 포인터가 가리키는 커밋 정보 확인

* `$ git show <커밋해시값>`   
특정 커밋 정보를 확

<br>

# 5. clone
* ```$ git clone [REPO_URL] [DIR]```   
[REPO_URL]에는 클론해올 저장소의 주소를 지정하고, [DIR] 인자는 저장소를 복제할 위치를 지정 (생략 가능)   

<br>

# 6. push & pull
$ git push   
$ git push [remote] [branch]   

$ git pull   
$ git pull [remote] [branch]   


# 7. fetch & merge
$ git fetch   
$ git merge [remote] [branch]   

<br>

# 8. branch
$ git branch
$ git branch -a
$ git branch [new-branch]
$ git branch -d [branch]
$ git branch -D [branch]

# 9. checkout
$ git checkout [branch]
$ git checkout -b [new-branch]
$ git checkout -

# 10. switch
$ git switch [branch]
$ git switch -c [new-branch]
$ git switch -

# 11. rebase
$ git rebase [branch]
$ git rebase --continue
$ git rebase --abort

# 12. reset revert
$ git reset --soft [commit ID]
$ git reset --mixed [commit ID]
$ git reset --hard [commit ID]
$ git reset --hard ORIG_HEAD
$ git revert [commit ID]
