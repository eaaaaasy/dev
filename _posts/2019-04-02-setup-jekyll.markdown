---
layout: post
title:  "github.io & Jekyll 2"
date:   2019-04-02 22:17:55 +0900
categories: jekyll github.io
---

<h3>github.io(블로그)를 만들면서 jekyll, git, github를 배워보자 1</h3>

두 개의 계정으로 작업을 한다. benah13yun, eaaaaasy<br/>
benah13yun은 사이트의 주인이며 eaaaaasy는 협력자이다.<br/>

<span style="color:red">
SVN처럼 다른 계정(eaaaaasy)으로 benah13yun의 저장소에 커밋 해보기 (X)<span>
<pre style='text-decoration:line-through;'>
git clone https://github.com/benah13yun/dev.git //가져왔다!
git add . // git에 추가한다?
git commit -m 'push test' // 메시지와 함께 커밋한다?

// 올리자! 내 경우엔 계정을 묻는다. 저장되어 있다면 안물을수도 있다.
git push origin master

이렇게 하면 되는 건 줄 알았다. 비슷하다며!!
</pre>

<span style="color:blue">
<br/>프로젝트 소유자가 반드시 있고, 프로젝트 소유자는 다른 사람들이 수정한 코드의 적용 여부를 결정한다.
<br/>
<br/>저장소를 내 github에 복사하고, 그것을 내 PC로 가져와서 수정한 다음, 프로젝트 소유자에게
<br/>" 이 코드 어때요? 쓸래요? " 라고 물어본다.
<br/>소유자는 쓸지말지 결정한다.
<br/>
<br/>여기까지 아래 코드~
</span>

<pre>
benah13yun 프로젝트 소유자, eaaaaasy 참여자
(eaaaaasy계정으로 하는 것이다.)

https://github.com/benah13yun/dev에 가서 fork를 누른다.
>> 이렇게 하면 내 저장소에 dev가 생성된다.

git clone https://github.com/eaaaaasy/dev
>> 내 컴퓨터에 다운 받는다.

git checkout -b 20190402ver2 //브랜치를 만든다.
>> 안만들어도 된다.

git commit -a -m 'little change' //커밋한다.

git push origin 20190402ver2 // 브랜치를 Push한다.
>> 브랜치를 안만들었으면 git push orgin master

https://github.com/eaaaaasy/dev
에서 (New) pull request 버튼을 눌러 소유자(benah13yun)에게 알린다.

benah13yun계정으로 로그인한다.
https://github.com/benah13yun/dev
에서 pull requests에서 merge pull request를 눌러 master에 병합한다.

conflict가 발생하면 merge버튼이 나오지 않는다.
해결 후 저장하면 나온다.
</pre>

<pre>

[참고]

git branch -l //브랜치 보기
git branch -d [branchName] //브랜치 지우기

https://git-scm.com/book/ko/v2/GitHub-GitHub-프로젝트에-기여하기

</pre>
