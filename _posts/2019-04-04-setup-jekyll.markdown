---
layout: post
title:  "github.io & Jekyll 3"
date:   2019-04-04 22:17:55 +0900
categories: jekyll github.io
---

<h3>github.io(블로그)를 만들면서 jekyll, git, github를 배워보자 3</h3>

<pre style="color:blue; background-color:#cccccc;">
두 개의 계정으로 만든다. // git을 배우려고.
jekyll은 기본 테마로 설치한다. // 천천히 하자.
공식사이트를 많이 보자. // 많이 봐야 친해진다.

**미리해두었다.**
1. benah13yun, eaaaaasy 두 개의 계정으로 github에 가입.
2. benah13yun으로 benah13yun.github.io/dev 리파지토리 생성.
</pre>

<span style="color:blue;">
다른 소유자의 원격저장소의 데이터를 내 로컬로 가져와보자. <b>clone 말고 pull~</b></span>
<pre>
프로젝트(benah13yun/dev)의 데이터를 eaaaaasy의 로컬(컴퓨터)에 받아와 보자.

로컬컴에 아무것도 없을 때는 
<b>git clone https://github.com/benah13yun/dev.git</b> 으로 가져왔다.
이건 내 로컬에 dev라는 디렉토리를 만드는 것 부터 시작한다.
지금은 로컬에 이미 받아둔게 있기 때문에 pull을 사용해서 받아와야 한다.

내 저장소의 데이터를 받아올땐 어떻게 했는지 기억해보자.
<b>git pull origin master</b>
그래 이렇게 했었다. 가 아니라 해본적이 없다... 어쩐지.
아무튼 위의 코드는 맞다. (강제 덮어쓰기는 -f 추가)

남의 저장소의 데이터를 내 로컬컴에 받아오는걸 할거니까.
<b>git pull https://github.com/benah13yun/dev master</b>
이렇게 하면 된다.

origin과 master가 뭔지 알고 있었다면 쉬웠을거다.

내 원격 저장소가 origin으로 지정되어있고, 다른 원격 저장소도 짧은 이름으로 지정할 수 있다.
<b>git remote add [shortName] [repository URL]</b>

<b>git remote add bena https://github.com/benah13yun/dev.git</b>
이렇게 bena라는 이름으로 저장했다.

<b>git pull bena master</b>
bena 를 master로 가져온다.

<b>git remote -v</b> //원격 저장소의 리스트를 보고 싶다!
bena    https://github.com/benah13yun/dev.git (fetch)
bena    https://github.com/benah13yun/dev.git (push)
origin  https://github.com/eaaaaasy/dev (fetch)
origin  https://github.com/eaaaaasy/dev (push)

</pre>

<pre>
*주의사항*
빈 디렉토리는 포함되지 않는다.
Head는 현재 브랜치의 가장 최신커밋을 의미함.
원격저장소의 이름은 origin이다.
</pre>

<pre>
<b>Git을 조금 더 알아보기 출처 https://git-scm.com/book/ko/v1/t시작하기-Git-기초</b>

Git은 파일을 세 가지 상태로 관리한다.
1. Committed (git commit)
 - 데이터가 로컬에 안전하게 저장되었다.
2. Modified
 - 수정한 파일이 커밋하지 않은 상태로 로컬에 있다.
3. Staged (git add)
 - 수정한 파일을 곧 커밋할 거라고 선언한 상태에 있다.

<b>Commands</b>

git add 스테이지 영역에 올린다.
<b>git add -p</b>

git commit 로컬저장소에 올린다.
<b>git commit -v</b>
git fetch 로컬저장소에서 받는다.

git push 원격저장소에 올린다.
<b>git push origin master</b>
git pull 원격저장소에서 받는다.
<b>git pull origin master</b>

git clone
git remote

옵션
-n, --dry-run : 테스트를 한다.
-v, --verbose : 한 번 더 확인한다. ?

config
git config --global user.name "userName"
git config --global user.email user@email.com

branch
git branch -l

</pre>