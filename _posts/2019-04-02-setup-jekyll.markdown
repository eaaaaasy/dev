---
layout: post
title:  "github.io & Jekyll 2"
date:   2019-04-02 22:17:55 +0900
categories: jekyll github.io
---

<h2>github.io를 만드는 과정을 작성한다.</h2>

jekyll을 사용한다. 읽기도 애매하고 하하의 지키리가 생각나기도 한다.<br/>
배우기가 번거롭지만 테마도 있고 다들 쓰는 이유가 있겠지 하는 마음에 사용한다.<br/>
(사실 여기까지 엄청 오랜 시간이 걸렸다. 뻘짓의 연속.)

<br/>
<a href='https://jekyllrb-ko.github.io/docs/windows/' target="_blank">
https://jekyllrb-ko.github.io/docs/windows/
</a> 여기를 참고하여 루비와 지킬을 설치한다.

루비의 설치가 끝나면 MSYS2의 설치를 묻는데 1, 2, 3 순서로 모두 설치한다.
{% highlight javascript %}
gem install jekyll bundler //설치 (시간이 좀 걸림)
jekyll -v //버전확인
> jekyll 3.x.x
jekyll new TITLE //설치 (오래 걸림)
cd TITLE
bundle exec jekyll serve //시작 localhost:4000
{% endhighlight %}
여기까지 하면 기본 블로그가 실행된다.
기본블로그가 깔끔하다.


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
