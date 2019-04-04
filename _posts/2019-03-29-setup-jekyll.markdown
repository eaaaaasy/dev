---
layout: post
title:  "github.io & Jekyll 1"
date:   2019-03-29 22:17:55 +0900
categories: jekyll github.io
---

<h3>github.io(블로그)를 만들면서 jekyll, git, github를 배워보자 1</h3>

<pre style="color:blue;">
두 개의 계정으로 만든다. // git을 배우려고.
jekyll은 기본 테마로 설치한다. // 천천히 하자.
공식사이트를 많이 보자. // 많이 봐야 친해진다.
</pre>

<pre>
**미리해두었다.**
1. benah13yun, eaaaaasy 두 개의 계정으로 github에 가입.
2. benah13yun으로 benah13yun.github.io/dev 리파지토리 생성.
</pre>

<br/>
<a href='https://jekyllrb-ko.github.io/docs/windows/' target="_blank">
https://jekyllrb-ko.github.io/docs/windows/
</a> 여기를 참고하여 루비와 지킬을 설치한다.
<br/>윈도우 기준이고 맥은 더 쉽다.

루비의 설치가 끝나면 MSYS2의 설치를 묻는데 1, 2, 3 순서로 모두 설치한다.
{% highlight javascript %}
gem install jekyll bundler //설치 (시간이 좀 걸림)
jekyll -v //버전확인
> jekyll 3.x.x
jekyll new TITLE //설치 (오래 걸림)
cd TITLE

git add .
git commit -m '내 블로그에요~'
git push origin master

bundle exec jekyll serve //시작 localhost:4000

{% endhighlight %}
여기까지 하면 github에 올라가고 로컬에서 기본 블로그가 실행된다.
기본블로그가 깔끔하다.
<br/>
[다음 글에는 git을 사용하여 github에 올리는 방법을 쓴다.]
[다음-글]


이하는 기본 블로그에 작성되어 있는 글이다. 참고용으로 남겨둔다.<br/>
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
[다음-글]: /dev/jekyll/github.io/2019/04/02/setup-jekyll.html