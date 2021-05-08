## github repository URL: *<http://github.com/seoseoseodabin/SE-assignment2>*

<br><br>

## **1. init**
![init](https://user-images.githubusercontent.com/68491776/117541262-ff78a880-b04d-11eb-861c-057584767d9b.PNG)

- 현재 프로젝트를 위한 디렉터리를 만든 상태이다.
- 이 디렉터리의 파일들을 버전관리하고 싶다.
- 이를 위해 git 명령어 'init'을 사용하였다.
- 'git init'은 디렉터리를 깃 저장소로 초기화해줄 때 사용하는 명령어이다. 'git init *[디렉터리 이름]*'은 디렉터리를 생성과 동시에 초기화해준다. 

<br>

## **2. config**
![config](https://user-images.githubusercontent.com/68491776/117541269-0d2e2e00-b04e-11eb-9062-94b69c89886d.PNG)

- 현재 깃 초기화를 진행한 상태이다.
- 어떤 버전을 누가 언제 만들었는지 확인할 수 있도록 사용자 정보를 입력하고 싶다.
- 이를 위해 git 명령어 'config'를 사용하였다.
- 'git config user.name'은 사용자의 이름을 입력하는 명령어이고, 'git config user.email'은 사용자의 이메일 정보를 입력하는 명령어이다. 아무 옵션 없이 사용하면 해당 저장소 내에서만 사용되고, '--global' 옵션을 추가하면 현재 컴퓨터에 있는 모든 저장소에서 사용된다.

<br>

## **3. add**
![add](https://user-images.githubusercontent.com/68491776/117541273-115a4b80-b04e-11eb-9f9c-9e7c66d80625.PNG)

- 현재 md_tutorial.md 파일을 만들고 markdown basic syntax의 1~4번 내용을 작성한 상태이다.
- 이 파일을 하나의 버전으로 만들고 싶다.
- 우선 커밋에 앞서 스테이징을 하기 위해 git 명령어 'add'를 사용하였다.
- 하나의 버전을 만들기 위해서는 스테이징 -> 커밋의 순서를 거쳐야 한다. 스테이징은 작업트리(현재 우리가 있는 디렉터리)에 있는 파일을 스테이지에 올리는 것을 얘기하는데, 스테이지는 버전으로 만들 파일들이 대기하는 곳이다.
- 'git add' 명령어 뒤에 버전으로 만들고 싶은 파일 이름을 입력하면 그 파일은 스테이지로 올라간다.

<br>

## **4. commit**
![commit](https://user-images.githubusercontent.com/68491776/117541280-17e8c300-b04e-11eb-931f-d11cde8b1540.PNG)

- 현재 md_tutorial.md 파일을 스테이지로 올린 상태이다.
- 이 파일을 버전으로 만들기 위해 커밋하고 싶다.
- 이를 위해 git 명령어 'commit'을 사용하였다.
- 저장소(repositery)는 스테이지에서 대기하고 있던 파일들을 버전으로 만들어 저장하는 곳이다. 스테이지에 있는 파일들을 저장소로 넘기기 위해서는(버전으로 만들기 위해서는) 'git commit' 명령어를 사용하면 된다.
- 자주 사용되는 옵션은 '-m'과 '-a'이다. '-m' 옵션을 사용하면 커밋할 때 메시지를 추가할 수 있고, '-a' 옵션을 사용하면 따로 스테이징 하지 않아도 된다. 단 '-a' 옵션은 한 번 커밋한 파일에 한해서 사용할 수 있다. 주로 '-am'의 형태로 자주 사용된다.

<br>

## **5. status**
![status](https://user-images.githubusercontent.com/68491776/117541286-22a35800-b04e-11eb-8f50-8416b0e4a93b.PNG)

- 현재 첫 번째 커밋을 완료한 상태이다.
- 내 깃 상태가 어떤지 확인하고 싶다.
- 이를 위해 git 명령어 'status'를 사용하였다.
- 'git status' 명령어를 사용하면 깃 상태를 알 수 있다. 현재 어떤 branch에 있는지, 작업 트리에 변화가 있었는지, 스테이지에 파일이 있는지 등의 정보를 알려준다.
- 위 사진에서는 현재 master 브랜치에 있고, 스테이지에 파일이 없으며(커밋할 파일이 없으며), 작업 트리가 최신 커밋과 비교해 아무 변화도 없다고 알려주고 있다.

<br>

## **6. remote**
![remote](https://user-images.githubusercontent.com/68491776/117541296-2df68380-b04e-11eb-802f-4b2755408615.PNG)

- 현재 첫 번째 버전을 만든 상태이다.
- 이 버전을 원격 저장소에 올리고 싶다.
- 이를 위해 우선 로컬 저장소와 원격 저장소를 연결하기 위해 git 명령어 'remote'를 사용하였다.
- 'git remote add origin *[원격 저장소 주소]*'를 입력하면 로컬 저장소와 원격 저장소가 연결된다. 이 작업은 처음 딱 한 번만 하면 된다.
- 현재 내 로컬 저장소가 어떤 원격 저장소와 연결되어 있는지 확인하기 위해서는 'git remote -v'를 사용하면 된다.

<br>

## **7. push**
![push](https://user-images.githubusercontent.com/68491776/117541304-3e0e6300-b04e-11eb-8ddb-c5775390c73d.PNG)

- 현재 첫 번째 버전을 만들었고, 로컬 저장소를 원격 저장소와 연결한 상태이다.
- 원격 저장소에 첫 번째 버전을 올리고 싶다.
- 이를 위해 git 명령어 'push'를 사용하였다.
- 원격 저장소에 버전을 올리려면 'git push'를 입력하면 된다. 사진에서는 'git push -u origin master'이라고 입력했는데, '-u' 옵션은 지역 저장소의 브랜치를 원격 저장소의 master 브랜치에 연결하기 위한 것이다. 이 작업은 처음 한 번만 하면 된다.

<br>

## **8. log**
![log](https://user-images.githubusercontent.com/68491776/117541326-567e7d80-b04e-11eb-9a3d-4f8aa10e03b3.PNG)

- 현재 첫 번째 커밋을 완료한 상태이다.
- 제대로 커밋이 됐는지 목록을 보고 싶다.
- 이를 위해 git 명령어 'log'를 사용하였다.
- 'git log'를 사용하면 현재까지의 커밋 내역을 보여준다. 여기에는 커밋메시지와 버전을 만든 사람와 날짜 정보가 함께 담겨있다. 'commit' 옆에 있는 긴 문자열은 '커밋 해시'로, 커밋을 구별하는 일종의 아이디 같은 것이다. 
- 커밋 해시 옆에 '(HEAD->master, origin/master)'라고 써 있는데, 이것은 이 커밋이 (로컬 저장소의) master 브랜치, origin(원격 저장소)의 master 브랜치의 최신 커밋이라는 의미이다. 또, 'HEAD->master'는 현재 작업 중인 브랜치가 master 브랜치라는 뜻이다. 참고로 master 브랜치는 깃 초기화 하자마자 생성되는 브랜치로 가장 기본적이고 특별한 브랜치이다.
- '--oneline'이라는 옵션을 추가하면 커밋을 한 줄에 한 커밋씩 나타난다.

<br>

## **9. reset**
![reset](https://user-images.githubusercontent.com/68491776/117541328-5a120480-b04e-11eb-8667-f48a1f52d4cb.PNG)
![reset2](https://user-images.githubusercontent.com/68491776/117541332-5da58b80-b04e-11eb-8694-580f19fdf320.PNG)

- md_tutorial.md 파일에 basic syntax의 5번 내용을 추가하려 했는데, 실수로 GFM의 syntax로 잘못 추가했다. 현재 "basic syntax 5"라는 커밋 메시지와 함께 커밋까지 하고 원격저장소로 push도 한 상태이다.
- 가장 최신 커밋을 삭제하고, md_tutorial.md 파일도 수정 전으로 되돌리고 싶다.
- 이를 위해 git 명령어 'reset'을 옵션 '--hard'와 함께 사용하였다.
- 'reset'은 reset 하고자 하는 커밋으로 돌아간 다음 해당 커밋 이후의 커밋들을 모두 다 삭제해주는 명령어이다. 'reset *옵션* *돌아가고자 하는 커밋해시*' 이런 식으로 사용한다. 가장 최신 커밋만 삭제할 때는 커밋해시 대신 'HEAD^'를 넣어도 된다. 옵션은 총 세 가지로 기능은 다음과 같다.

|옵션|기능|
|:--:|:--|
|--soft *커밋 해시*|해당 커밋 이후의 커밋들을 삭제. 하지만 스테이지에는 남아 있으므로 바로 커밋하면 복구할 수 있음|
|--mixed *커밋 해시*|커밋과 스테이징을 하기 전 상태로 되돌림. 바로 스테이징과 커밋을 하면 복구할 수 있음. 옵션 없이 reset 명령어를 실행하면 이 옵션이 기본으로 적용됨.|
|--hard *커밋 해시*|커밋과 스테이징, 파일 수정을 하기 전 상태로 되돌림. 이 옵션으로 실행하면 절대 다시 복구할 수 없음.|

<br>

![push--force](https://user-images.githubusercontent.com/68491776/117541343-68602080-b04e-11eb-8637-9e59fe595179.PNG)

- 원격 저장소에도 반영하고 싶은데, reset 명령은 시간을 되돌린 거나 다름 없기 때문에 이대로 'git push' 명령어를 실행하면 오류가 난다. 따라서 강제로 push 하게 해주는 옵션 '-f'나 '--force'를 추가해서 실행해주어야 한다.
- reset 명령어는 커밋 이력을 아예 삭제해주기 때문에 혼자만 사용하는 브랜치가 아닐 경우 사용을 매우매우 조심해야 한다. (다른 사람들의 로컬 저장소에는 커밋 내용이 남아있을 수 있으므로)

<br>

## **10. clone**
![clone](https://user-images.githubusercontent.com/68491776/117541352-74e47900-b04e-11eb-802a-c509bd67fc76.PNG)

- 현재 md_tutorial.md 파일에 basic syntax의 5~6번 내용을 추가하고 커밋, 원격 저장소로 push까지 완료한 상태이다. 지금까지 컴퓨터에서 작업하고 있었는데 갑자기 사정이 생겨 임시로 다른 컴퓨터에서 작업해야 하는 상황이다.
- 지금까지의 작업 내용을 그대로 다른 컴퓨터로 옮기고 싶다.
- 이를 위해 git 명령어 'clone'을 사용하였다.
- 원격 저장소를 다른 로컬 저장소에서 사용하기 위해서는 원격 저장소의 내용을 복제해와야 하는데, 이때 사용하는 명령어가 'git clone *[원격 저장소 주소]* *[복제할 디렉터리 이름]*'이다. 이떄 파일이 없으면 새로 만들어준다. 또한 따로 초기화 해줄 필요 없다.
- (꾸며낸 상황이라 다른 컴퓨터에서 작업하는 대신 다른 디렉터리를 새로 만들어 작업하는 것으로 대체했습니다.)

<br>

## **11. rebase**
![basicsyntax7~12](https://user-images.githubusercontent.com/68491776/117541359-7ada5a00-b04e-11eb-800c-e2693fccecec.PNG)
![rebase](https://user-images.githubusercontent.com/68491776/117541366-80d03b00-b04e-11eb-9062-3b92841ce5db.PNG)
![rebase2](https://user-images.githubusercontent.com/68491776/117541369-83cb2b80-b04e-11eb-9339-e8661d73615b.PNG)

- 현재 clone으로 복제한 디렉터리에서 작업 중이고, basic syntax 7~12번 내용까지 추가하였다. 내용을 추가하는 족족 커밋과 push까지 해서 총 5개의 커밋이 새로 추가되었다. (첫번째 사진 참조)
- 너무 지저분해 이 다섯 개의 커밋을 하나로 합치고 싶다.
- 이를 위해 '-i' 옵션과 함께 git 명령어 'rebase'를 사용하였다.
- 'rebase'는 커밋 내역을 수정하고 싶을 때, 브랜치를 병합하고 싶을 때 사용한다. 내가 사용한 경우는 전자에 속한다.
- 커밋 내역을 수정할 때는 'rebase -i HEAD~*[숫자]*' 이 명령어를 쓴다. 여기서 *숫자*는 커밋 내역을 수정하는 데에 고려할 커밋의 개수를 의미힌다. 이 명령어를 입력하면 창이 하나 뜨는데, 보면 커밋 해시 앞에 pick이라고 적혀있다. 수정하고 싶은 커밋의 pick을 어떤 알파벳으로 바꾸느냐에 따라 할 수 있는 작업이 달라진다.

    |명령어|기능|
    |:---:|:--|
    |reword|커밋 메시지 변경|
    |edit|커밋 메시지 + 작업 내용 변경|
    |squash|해당 커밋을 이전 커밋과 합침|
    |fixup|해당 커밋을이전 커밋과 합치지만 메시지는 합치지 않음. 이전 커밋 메시지만 남게 됨|
    |drop|커밋 히스토리에서 커밋 삭제|  
    
<br>

- 나는 여러 커밋을 하나로 합칠 것이기 때문에 가장 최신 커밋부터 4개까지의 커밋 앞의 pick을 's(squash)'로 바꿔주었다. 바꾼다음 저장하고 종료하면, 4개의 커밋이 바로 이전 커밋으로 녹아들어간다. 이때 커밋 메시지를 수정할 수 있는 창이 뜨는데, 거기서 커밋 메시지를 수정해주면 된다.
- 'rebase'를 사용하면 충돌이 발생할 수도 있다. 이때에는 창이 뜨는데, 거기서 충돌을 해결해주면 된다. 파일이 여러 개일 경우에는 'git rebase --continue'를 통해 다른 파일들에 충돌이 남아 있지 않은지 확인해주어야 한다. 만일 rebase 전으로 돌아가고 싶다면 'git rebase --abort'를 입력해주면 된다.
- rebase 명령어는 과거 시점으로 돌아가 다시 커밋 내역을 쌓는 느낌의 명령어이기 때문에, 그냥 push할 경우 기존의 커밋 내역과 엉켜 push가 안 될 수도 있다. 그렇기 때문에 '-f'나 '--force' 옵션을 넣어 강제로 push 시켜줘야 한다. 한 번 push로 내보낸 커밋에 대해서는 사용하지 않는 것이 좋다.

<br>

## **12. pull**
![pull](https://user-images.githubusercontent.com/68491776/117541372-8a59a300-b04e-11eb-8433-04b46843ebe4.PNG)

- 현재 처음부터 작업하던 디렉터리로 돌아온 상태이고, 원격 저장소의 md_tutorial.md 파일은 basic syntax 12번까지 작성되어 있고, 로컬 저장소의 md_tutorial.md 파일은 6번까지 작성되어 있다.
- 로컬 작업소에 원격 저장소의 작업 내역을 가져오고 싶다.
- 이를 위해 git 명령어 'pull'을 사용하였다.
- 'pull'명령어는 로컬 저장소에 원격 저장소의 커밋 내역을 내려받을 때 사용하는 명령어이다. 'git pull *[원격 저장소]* *[가져올 브랜치]*'이런 식으로 사용하면 된다. 'git pull origin master'일 때는 'git pull'이라고만 입력해도 된다.

<br>

## **13. branch**
![branch](https://user-images.githubusercontent.com/68491776/117541376-8ded2a00-b04e-11eb-8293-71d8b60bbbef.PNG)

- 현재 basic syntax의 내용은 12번까지 다 작성한 상태이고, 추가로 위에 인덱스를 넣어주었다.
- 인덱스에 heading id를 넣고 싶은데, 지금 파일은 그대로 두고 이걸 복사한 다른 파일을 만들어 거기서 작업하고 싶다. 잘 동작하면 그때 수정하고 싶다.
- 이를 위해 git 명령어 'branch'를 사용하였다.
- branch는 말 그대로 분기를 의미한다. branch 명렁어를 실행하면 그 시점의 커밋을 베이스로 분기가 만들어지기 때문에 따로 복사할 필요 없이 작업을 분리할 수 있다.
- 'git branch *[브랜치 이름]*'의 형태로 입력하면 브랜치가 만들어진다. 현재 어떤 브랜치가 있는지 확인할 때는 'git branch'만 입력하면 된다.

<br>

## **14. checkout**
![checkout](https://user-images.githubusercontent.com/68491776/117541380-9180b100-b04e-11eb-909f-9381d70c141d.PNG)

- 현재 basic syntax의 내용은 12번까지 다 작성한 상태이고, 추가로 위에 인덱스를 넣어주었고, heading_id라는 브랜치를 만든 상태이다.
- heading_id 브랜치로 옮겨서 작업하고 싶다.
- 이를 위해 git 명령어 'checkout'을 사용하였다.
- 'git checkout *[이동할 브랜치 이름]*'을 입력하면 해당 브랜치로 이동할 수 있다. 참고로, 이때 git log 명령어를 실행해보면 HEAD가 해당 브랜치를 가리키고 있는 것을 볼 수 있다. HEAD는 현재 작업하고 있는 브랜치를 가리키고 있는 일종의 포인터이다.
- checkout에는 이것 외에 다른 기능도 있는데, 'git checkout *--[파일 이름]*'을 입력하면 파일이 modified 되기 전으로 돌려준다.

<br>

## **15. merge**
![merge](https://user-images.githubusercontent.com/68491776/117541385-9d6c7300-b04e-11eb-9818-cf4792fe4813.PNG)

- 현재 heading_id 브랜치에서 md_tutorial.md 파일의 인덱스에 heading id를 넣은 상태이다.
- master 브랜치에 heading_id 브랜치의 내용을 가져오고 싶다.
- 이를 위해 git 명령어 'merge'를 사용하였다.
- merge는 브랜치들을 병합할 때 사용하는 명령어이다. 우선 병합을 진행할 브랜치로 이동한 후 'git merge *[병합할 브랜치 이름]*'을 입력하면 된다.
- merge하는 과정 중에 충돌이 발생할 수도 있다. 충돌이 발생하면 창이 하나 뜨는데, 그 창에서 해결하면 된다.
- 브랜치가 성공적으로 병합되면 새로운 커밋이 생긴다. 이때 커밋 메시지를 수정할 수 있는 창이 하나 뜨는데, 커밋 메시지를 수정하고 싶다면 그 창에서 수정하면 된다.
- 사진을 보면 Fast-forward라는 글씨가 보인다. 빨리 감기 병합이라고 하는데, master 브랜치에서 새로운 브랜치를 분기한 후에 master 브랜치에 아무 새로운 커밋도 없을 경우 일어난다. 이런 경우 브랜치를 병합하는 것이 쉽기 때문에 따로 커밋이 생기지 않는다.

<br>

## **16. tag**
![tag](https://user-images.githubusercontent.com/68491776/117541389-a52c1780-b04e-11eb-90ca-164d30af8f90.PNG)

- 현재 basic syntax 12번까지 다 작성했고, 인덱스에 heading id도 추가한 상태이다.
- 지금까지 프로젝트를 하는 과정 중에 여러 버전이 생겼다. 그렇지만 결과적으로 봤을 때 지금 이 버전이 완성된 하나의 버전이기 때문에 이를 나타내고 싶다.
- 이를 위해 git 명령어 'tag'를 사용하였다.
- tag는 한 마디로 특정 커밋에 붙이는 이름표 같은 것이다. HEAD가 최신 커밋을 가리키는 포인터라고 한다면, tag는 특정 커밋을 가리키는 고정된 포인터라고 할 수 있다. 'git tag *[태그 이름]* *[태그로 만들 커밋 해시]*'를 입력하면 해당 커밋에 태그를 붙일 수 있다.
-'git tag'를 입력하면 전체 태그를 조회할 수 있고 'git tag -v *[태그 이름]*'를 입력하면 특정 태그를 조회할 수 있다.
- 태그를 push할 때는 '--tags' 옵션을 추가해주어야 한다.
- 주로 릴리즈 버전을 나타낼 때 사용한다.

<br><br>

|명령어 목록|사용여부|
|:--------:|:------:|
|[init](#1-init)|O|
|[config](#2-config)|O|
|[add](#3-add)|O|
|[commit](#4-commit)|O|
|[status](#5-status)|O|
|[remote](#6-remote)|O|
|[push](#7-push)|O|
|[log](#8-log)|O|
|[reset](#9-reset)|O|
|[clone](#10-clone)|O|
|[rebase](#11-rebase)|O|
|[pull](#12-pull)|O|
|[branch](#13-branch)|O|
|[checkout](#14-checkout)|O|
|[merge](#15-merge)|O|
|[tag](#16-tag)|O|
