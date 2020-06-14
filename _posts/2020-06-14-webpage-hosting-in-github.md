This post describes how to host a website/blog using the [minimal-mistake theme](https://github.com/mmistakes/minimal-mistakes).



Fork/clone github repository `https://github.com/mmistakes/minimal-mistakes` in your github account.

```bash
git clone https://github.com/mmistakes/minimal-mistakes
cd minimal-mistakes

# remore default files
sudo git rm .editorconfig .gitattributes .github CHANGELOG.md\
		minimal-mistakes-jekyll.gemspec README.md \
		screenshot-layouts.png screenshot.png 
sudo git rm -rf .github docs test 

#content of Gemfile as like below
$ cat Gemfile
source "https://rubygems.org"
gem "jekyll", "~> 3.5"
gem "minimal-mistakes-jekyll"
$

#install necessary dependency
sudo bundle install

#check website localy 
sudo bundle exec jekyll serve

#update pages
sudo bundle update

#push changes to github repository  
```

