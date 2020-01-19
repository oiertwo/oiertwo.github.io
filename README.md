

### My PETsornal website
Theme based in [devlopr-jekyll](https://github.com/sujaykundu777/devlopr-jekyll)


### Setting up Development Environment

Step 1 - Clone your repo locally

```
git clone <repo.git>
```
Step 2 - Install Ruby and Bundler

We need ruby and Bundler to build our site locally.

Install Ruby

```
ruby -v
ruby 2.5.1p57 (2018-03-29 revision 63029) [x86_64-linux-gnu]
```

Install Bundler

```
gem install bundler
```

After installation check if its working:

```
bundler -v
Bundler version 2.0.1
```

Step 3 - Install the dependencies

```
$ bundle update
$ bundle install
```

Step 4 - Serve the site locally (development mode)

```
$ bundle exec jekyll serve
```

Webpage should be running in http://localhost:4000 


### Making changes

Open the files using your favourite text editor and edit the files you want:

```
$ cd <repo.git>
$ atom .
```

    _config.yml file - replace with your own details
    _posts - Add your blog posts here
    _includes - You can replace the contents of the files with your data. (contains widgets)
    _assets/img - Add all your images here


You can visit the site at http://localhost:4000 using ```bundle exec jekyll serve``` command.


Publish Your Changes:

```
$ cd yourusername.github.io
$ git add .
$ git commit -m "made changes to my blog"
$ git push 
```

### Run using Docker 

```
$ git clone 
$ cd repo
$ export JEKYLL_VERSION=3.8
$ docker run --rm --volume="$PWD" -it jekyll/jekyll:$JEKYLL_VERSION jekyll build
$ jekyll serve
```

### Licence

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).



