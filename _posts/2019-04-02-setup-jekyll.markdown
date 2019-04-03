---
layout: post
title:  "github.io & Jekyll 2"
date:   2019-04-02 22:17:55 +0900
categories: jekyll github.io
---

<h2>github.io를 만드는 과정을 작성한다. 2</h2>
{% highlight javascript %}
{% endhighlight %}

<h2>다른 계정으로 가져와서 push 해보기 (X)</h2>
<h2>GitHub 프로젝트에 기여하기 (O)</h2>
<h2>Team GitHub 프로젝트에 참여하기 (O)</h2>

<pre style='background-color:red'>
git clone https://github.com/benah13yun/dev.git //가져왔다!
올려보자.
git add .
git commit -m 'push test'
git push origin master

이렇게 하면 다른 계정으로도 benah13yun/dev의 master에 push할 수 있는 건지 알았어. 하하하하하...
</pre>

<pre>
https://github.com/benah13yun/dev에 가서 fork를 누른다.
git clone https://github.com/ANT_USERNAME/dev
git checkout -b 20190402ver2 //브랜치를 만든다.
git commit -a -m 'little change' //커밋한다.
git push origin 20190402ver2 // 브랜치를 Push한다.

github에서 pull request 버튼을 눌러 소유자(benah13yun)에게 알린다.
소유자는 pull requests에서 merge pull request를 눌러 master에 병합한다.
물론 안할수도 있다.
</pre>

<pre>

[참고]

git branch -l
git branch -d [branchName]

https://git-scm.com/book/ko/v2/GitHub-GitHub-프로젝트에-기여하기

</pre>
