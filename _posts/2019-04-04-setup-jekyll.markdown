---
layout: post
title:  "github.io & Jekyll 3"
date:   2019-04-04 22:17:55 +0900
categories: jekyll github.io
---

<h3>github.io(블로그)를 만들면서 jekyll, git, github를 배워보자 3</h3>

<pre>
원래 프로젝트(benah13yun/dev)의 데이터를 eaaaaasy의 로컬(컴퓨터)에 받아와 보자.

로컬컴에 아무것도 없을 때는 
git clone https://github.com/benah13yun/dev.git 으로 가져왔다.
이건 내 로컬에 dev라는 디렉토리를 만드는 것 부터 시작한다.
지금은 로컬에 이미 받아둔게 있기 때문에 pull을 사용해서 받아와야 한다.

내 저장소의 데이터를 받아올땐 어떻게 했는지 기억해보자.
git pull origin master
그래 이렇게 했었다. 가 아니라 해본적이 없다... 어쩐지.
아무튼 위의 코드는 맞다. (강제 덮어쓰기는 -f 추가)

남의 저장소의 데이터를 내 로컬컴에 받아오는걸 할거니까.
git pull https://github.com/benah13yun/dev master
이렇게 하면 된다.

origin과 master가 뭔지 알고 있었다면 쉬웠을거다.

내 원격 저장소가 origin으로 지정되어있고, 다른 원격 저장소도 짧은 이름으로 지정할 수 있다.
git remote add [shortName] [repository URL]

나는 git remote add bena https://github.com/benah13yun/dev.git
이렇게 bena라는 이름으로 저장했다.

git remote -v //원격 저장소의 리스트를 보고 싶다!
bena    https://github.com/benah13yun/dev.git (fetch)
bena    https://github.com/benah13yun/dev.git (push)
origin  https://github.com/eaaaaasy/dev (fetch)
origin  https://github.com/eaaaaasy/dev (push)

</pre>

<pre>
git 명령어를 정리한다.

*주의사항*
빈 디렉토리는 포함되지 않는다.
Head는 현재 브랜치의 가장 최신커밋을 의미함.
원격저장소의 이름은 origin이다.

공통옵션
-n, --dry-run : 테스트를 한다.
-v, --verbose : 한 번 더 확인한다. ?

</pre>
<pre>
Commands

git add

git commit 로컬저장소에 올린다.
git fetch 로컬저장소에서 받는다.

git push 원격저장소에 올린다.
git pull 원격저장소에서 받는다.

git clone
git remote
</pre>