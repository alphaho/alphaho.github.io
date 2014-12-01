---
layout: post
title: Things about writing a blog in Github under username.github.io
---


##how to test the pages on localhost
Run `jekyll serve`[^1]

And it will auto regenerate the pages if you have modify any of the posts.

##how to put the github pages under url \<username>.github.io rather than \<username>.github.io/\<project-name>
Create a repository name as \<username>.github.io \(replace \<username> with yours). And push the changes to main branch rather than gh-pages branch.

##Enable footnotes under jekyll
in `_config.jml`, set `markdown` as `markdown: kramdown`.


Reference:  

- <http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html> \(in Chinese)
- <http://jekyllrb.com/docs/github-pages/>


P.S.:

[^1]: To install jekyll, use ruby gem: `gem install jekyll`